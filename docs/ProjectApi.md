# ProjectApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectDestroy**](#projectdestroy) | **DELETE** /api/v1/projects/{id} | Project@destroy|
|[**projectGetAllUsersFlagProjectByUserId**](#projectgetallusersflagprojectbyuserid) | **GET** /api/v1/projects/{projectId}/all_users/{userId} | Get all users by projectID and userID|
|[**projectGetProjectByIdAndOrganisationId**](#projectgetprojectbyidandorganisationid) | **GET** /api/v1/projects/{projectId}/organisations/{organisationId} | Get project details by projectID and organisationID|
|[**projectGetProjectByIdAndUserId**](#projectgetprojectbyidanduserid) | **GET** /api/v1/projects/{projectId}/users/{userId} | Get project details by projectID and userID|
|[**projectGetProjectUsers**](#projectgetprojectusers) | **GET** /api/v1/projects/{id}/users | Project@getProjectUsers|
|[**projectGetProjectUsersByOrganisationId**](#projectgetprojectusersbyorganisationid) | **GET** /api/v1/projects/{projectId}/organisations/{organisationId}/users | Get all users by projectID and organisationID|
|[**projectIndex**](#projectindex) | **GET** /api/v1/projects | Project@index|
|[**projectMakePrimaryContact**](#projectmakeprimarycontact) | **PUT** /api/v1/projects/{id}/users/{registryId}/primary_contact | Project@edit|
|[**projectShow**](#projectshow) | **GET** /api/v1/projects/{id} | Project@show|
|[**projectStore**](#projectstore) | **POST** /api/v1/projects | Project@store|
|[**projectUpdate**](#projectupdate) | **PUT** /api/v1/projects/{id} | Project@update|
|[**projectUpdateAllProjectUsers**](#projectupdateallprojectusers) | **PUT** /api/v1/projects/{id}/all_users | Project@updateAllProjectUsers|

# **projectDestroy**
> AffiliationDestroy200Response projectDestroy()

Delete a Project entry from the system

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let id: number; //Project entry ID (default to undefined)

const { status, data } = await apiInstance.projectDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Project entry ID | defaults to undefined|


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

# **projectGetAllUsersFlagProjectByUserId**
> ProjectGetAllUsersFlagProjectByUserId200Response projectGetAllUsersFlagProjectByUserId()

Fetches users for a project.

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let userId: number; //ID of the user (default to undefined)
let projectId: number; //ID of the project (default to undefined)

const { status, data } = await apiInstance.projectGetAllUsersFlagProjectByUserId(
    userId,
    projectId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **projectId** | [**number**] | ID of the project | defaults to undefined|


### Return type

**ProjectGetAllUsersFlagProjectByUserId200Response**

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
|**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectGetProjectByIdAndOrganisationId**
> CustodiansGetOrganisationUsers200Response projectGetProjectByIdAndOrganisationId()

Fetches project given organisation and project IDs.

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let organisationId: number; //ID of the organisation (default to undefined)
let projectId: number; //ID of the project (default to undefined)

const { status, data } = await apiInstance.projectGetProjectByIdAndOrganisationId(
    organisationId,
    projectId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationId** | [**number**] | ID of the organisation | defaults to undefined|
| **projectId** | [**number**] | ID of the project | defaults to undefined|


### Return type

**CustodiansGetOrganisationUsers200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successfully retrieved project |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Project not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectGetProjectByIdAndUserId**
> ProjectGetProjectByIdAndUserId200Response projectGetProjectByIdAndUserId()

Fetches project given user and project IDs.

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let userId: number; //ID of the user (default to undefined)
let projectId: number; //ID of the project (default to undefined)

const { status, data } = await apiInstance.projectGetProjectByIdAndUserId(
    userId,
    projectId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userId** | [**number**] | ID of the user | defaults to undefined|
| **projectId** | [**number**] | ID of the project | defaults to undefined|


### Return type

**ProjectGetProjectByIdAndUserId200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successfully retrieved project |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Project not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectGetProjectUsers**
> ProjectGetProjectUsers200Response projectGetProjectUsers()

Return project users by project ID

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let id: number; //Project entry ID (default to undefined)

const { status, data } = await apiInstance.projectGetProjectUsers(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Project entry ID | defaults to undefined|


### Return type

**ProjectGetProjectUsers200Response**

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

# **projectGetProjectUsersByOrganisationId**
> CustodiansGetOrganisationUsers200Response projectGetProjectUsersByOrganisationId()

Fetches users given organisation and project IDs.

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let organisationId: number; //ID of the organisation (default to undefined)
let projectId: number; //ID of the project (default to undefined)

const { status, data } = await apiInstance.projectGetProjectUsersByOrganisationId(
    organisationId,
    projectId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationId** | [**number**] | ID of the organisation | defaults to undefined|
| **projectId** | [**number**] | ID of the project | defaults to undefined|


### Return type

**CustodiansGetOrganisationUsers200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successfully retrieved organisation users |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Organisation users not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectIndex**
> ProjectIndex200Response projectIndex()

Return a list of Projects

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

const { status, data } = await apiInstance.projectIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**ProjectIndex200Response**

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

# **projectMakePrimaryContact**
> ProjectMakePrimaryContact200Response projectMakePrimaryContact(projectMakePrimaryContactRequest)

Make user a primary contact

### Example

```typescript
import {
    ProjectApi,
    Configuration,
    ProjectMakePrimaryContactRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let id: number; //Project entry ID (default to undefined)
let registryId: number; //Registry ID (default to undefined)
let projectMakePrimaryContactRequest: ProjectMakePrimaryContactRequest; //Project definition

const { status, data } = await apiInstance.projectMakePrimaryContact(
    id,
    registryId,
    projectMakePrimaryContactRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectMakePrimaryContactRequest** | **ProjectMakePrimaryContactRequest**| Project definition | |
| **id** | [**number**] | Project entry ID | defaults to undefined|
| **registryId** | [**number**] | Registry ID | defaults to undefined|


### Return type

**ProjectMakePrimaryContact200Response**

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

# **projectShow**
> ProjectIndex200Response projectShow()

Return a Project entry by ID

### Example

```typescript
import {
    ProjectApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let id: number; //Project entry ID (default to undefined)

const { status, data } = await apiInstance.projectShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Project entry ID | defaults to undefined|


### Return type

**ProjectIndex200Response**

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

# **projectStore**
> AccreditationStoreByRegistryId201Response projectStore(projectStoreRequest)

Create a Project entry

### Example

```typescript
import {
    ProjectApi,
    Configuration,
    ProjectStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let projectStoreRequest: ProjectStoreRequest; //Project definition

const { status, data } = await apiInstance.projectStore(
    projectStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectStoreRequest** | **ProjectStoreRequest**| Project definition | |


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
|**404** | Not found response |  -  |
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectUpdate**
> ProjectUpdate200Response projectUpdate(projectIndex200ResponseData)

Update a Project entry

### Example

```typescript
import {
    ProjectApi,
    Configuration,
    ProjectIndex200ResponseData
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let id: number; //Project entry ID (default to undefined)
let projectIndex200ResponseData: ProjectIndex200ResponseData; //Project definition

const { status, data } = await apiInstance.projectUpdate(
    id,
    projectIndex200ResponseData
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectIndex200ResponseData** | **ProjectIndex200ResponseData**| Project definition | |
| **id** | [**number**] | Project entry ID | defaults to undefined|


### Return type

**ProjectUpdate200Response**

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

# **projectUpdateAllProjectUsers**
> ONSSubmissionReceiveCSV200Response projectUpdateAllProjectUsers(projectUpdateAllProjectUsersRequest)

Update all users associated with a project

### Example

```typescript
import {
    ProjectApi,
    Configuration,
    ProjectUpdateAllProjectUsersRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectApi(configuration);

let id: number; //Project entry ID (default to undefined)
let projectUpdateAllProjectUsersRequest: ProjectUpdateAllProjectUsersRequest; //Project definition

const { status, data } = await apiInstance.projectUpdateAllProjectUsers(
    id,
    projectUpdateAllProjectUsersRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectUpdateAllProjectUsersRequest** | **ProjectUpdateAllProjectUsersRequest**| Project definition | |
| **id** | [**number**] | Project entry ID | defaults to undefined|


### Return type

**ONSSubmissionReceiveCSV200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success response |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

