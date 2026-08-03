# ProjectRoleApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**projectRoleIndex**](#projectroleindex) | **GET** /api/v1/project_roles | ProjectRole@index|
|[**projectRoleShow**](#projectroleshow) | **GET** /api/v1/project_roles/{id} | ProjectRole@show|
|[**projectRoleStore**](#projectrolestore) | **POST** /api/v1/project_roles | ProjectRole@store|
|[**projectRoleUpdate**](#projectroleupdate) | **PUT** /api/v1/project_roles/{id} | ProjectRole@update|

# **projectRoleIndex**
> ProjectRoleIndex200Response projectRoleIndex()

Return a list of ProjectRole

### Example

```typescript
import {
    ProjectRoleApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectRoleApi(configuration);

const { status, data } = await apiInstance.projectRoleIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**ProjectRoleIndex200Response**

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

# **projectRoleShow**
> ProjectRoleIndex200Response projectRoleShow()

Return a ProjectRole

### Example

```typescript
import {
    ProjectRoleApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectRoleApi(configuration);

let id: number; //ProjectRole entry ID (default to undefined)

const { status, data } = await apiInstance.projectRoleShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ProjectRole entry ID | defaults to undefined|


### Return type

**ProjectRoleIndex200Response**

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

# **projectRoleStore**
> IdentityStore201Response projectRoleStore(projectRole)

Create a ProjectRole

### Example

```typescript
import {
    ProjectRoleApi,
    Configuration,
    ProjectRole
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectRoleApi(configuration);

let projectRole: ProjectRole; //ProjectRole definition

const { status, data } = await apiInstance.projectRoleStore(
    projectRole
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectRole** | **ProjectRole**| ProjectRole definition | |


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
|**201** | Success |  -  |
|**404** | Not found response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projectRoleUpdate**
> ProjectRoleUpdate200Response projectRoleUpdate(projectRole)

Update a ProjectRole entry

### Example

```typescript
import {
    ProjectRoleApi,
    Configuration,
    ProjectRole
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProjectRoleApi(configuration);

let id: number; //ProjectRole entry ID (default to undefined)
let projectRole: ProjectRole; //ProjectRole definition

const { status, data } = await apiInstance.projectRoleUpdate(
    id,
    projectRole
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **projectRole** | **ProjectRole**| ProjectRole definition | |
| **id** | [**number**] | ProjectRole entry ID | defaults to undefined|


### Return type

**ProjectRoleUpdate200Response**

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

