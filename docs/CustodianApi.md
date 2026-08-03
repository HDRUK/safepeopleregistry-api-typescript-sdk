# CustodianApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianAddProject**](#custodianaddproject) | **POST** /api/v1/custodians/{custodianId}/projects | Custodian@addProject|
|[**custodianDestroy**](#custodiandestroy) | **DELETE** /api/v1/custodians/{id} | Custodian@destroy|
|[**custodianGetOrganisations**](#custodiangetorganisations) | **GET** /api/v1/custodian/{custodianId}/organisations | Return all custodian organisations with projects|
|[**custodianGetProjects**](#custodiangetprojects) | **GET** /api/v1/custodian/{custodianId}/projects | Return all projects associated with a custodian|
|[**custodianGetProjectsUsers**](#custodiangetprojectsusers) | **GET** /api/v1/custodians/{custodianId}/projects_users | Get all users associated with custodian\&#39;s projects|
|[**custodianGetUserProjects**](#custodiangetuserprojects) | **GET** /api/v1/custodian/{custodianId}/users/{userId}/projects | Return all custodian projects associated with a user|
|[**custodianIndex**](#custodianindex) | **GET** /api/v1/custodians | Custodian@index|
|[**custodianShow**](#custodianshow) | **GET** /api/v1/custodians/{id} | Custodian@show|
|[**custodianShowByUniqueIdentifier**](#custodianshowbyuniqueidentifier) | **GET** /api/v1/custodians/identifier/{id} | Custodian@showByUniqueIdentifier|
|[**custodianStore**](#custodianstore) | **POST** /api/v1/custodians | Custodian@store|
|[**custodianUpdate**](#custodianupdate) | **PUT** /api/v1/custodians/{id} | Custodian@update|

# **custodianAddProject**
> CustodianAddProject201Response custodianAddProject(custodianAddProjectRequest)

Create a project for a custodian

### Example

```typescript
import {
    CustodianApi,
    Configuration,
    CustodianAddProjectRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let custodianAddProjectRequest: CustodianAddProjectRequest; //Project definition

const { status, data } = await apiInstance.custodianAddProject(
    custodianId,
    custodianAddProjectRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianAddProjectRequest** | **CustodianAddProjectRequest**| Project definition | |
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**CustodianAddProject201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianDestroy**
> AffiliationDestroy200Response custodianDestroy()

Delete a Custodian entry from the system

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let id: number; //Custodian entry ID (default to undefined)

const { status, data } = await apiInstance.custodianDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Custodian entry ID | defaults to undefined|


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
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianGetOrganisations**
> CustodianGetOrganisations200Response custodianGetOrganisations()

Fetch a list of custodians organisations with projects, along with pagination details.

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let custodianId: number; //The ID of the custodian whose organisations are to be retrieved (default to undefined)

const { status, data } = await apiInstance.custodianGetOrganisations(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | The ID of the custodian whose organisations are to be retrieved | defaults to undefined|


### Return type

**CustodianGetOrganisations200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianGetProjects**
> CustodianGetProjects200Response custodianGetProjects()

Fetch a list of projects along with pagination details for a specified custodian.

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let custodianId: number; //The ID of the custodian whose projects are to be retrieved (default to undefined)

const { status, data } = await apiInstance.custodianGetProjects(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | The ID of the custodian whose projects are to be retrieved | defaults to undefined|


### Return type

**CustodianGetProjects200Response**

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
|**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianGetProjectsUsers**
> CustodianGetProjectsUsers200Response custodianGetProjectsUsers()

Returns paginated users for all projects under a specific custodian.

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let custodianId: number; //Custodian ID (default to undefined)

const { status, data } = await apiInstance.custodianGetProjectsUsers(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | Custodian ID | defaults to undefined|


### Return type

**CustodianGetProjectsUsers200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | List of users |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianGetUserProjects**
> CustodianGetUserProjects200Response custodianGetUserProjects()

Fetch a list of custodians projects associated with a user, along with pagination details.

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let custodianId: number; //The ID of the custodian whose projects are to be retrieved (default to undefined)
let userId: number; //The ID of the user whose projects are to be retrieved (default to undefined)

const { status, data } = await apiInstance.custodianGetUserProjects(
    custodianId,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | The ID of the custodian whose projects are to be retrieved | defaults to undefined|
| **userId** | [**number**] | The ID of the user whose projects are to be retrieved | defaults to undefined|


### Return type

**CustodianGetUserProjects200Response**

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
|**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianIndex**
> CustodianIndex200Response custodianIndex()

Return a list of Custodians

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

const { status, data } = await apiInstance.custodianIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CustodianIndex200Response**

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

# **custodianShow**
> CustodianIndex200Response custodianShow()

Return an Custodian entry by ID

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let id: number; //Custodian ID (default to undefined)

const { status, data } = await apiInstance.custodianShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Custodian ID | defaults to undefined|


### Return type

**CustodianIndex200Response**

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

# **custodianShowByUniqueIdentifier**
> CustodianIndex200Response custodianShowByUniqueIdentifier()

Return an Custodian entry by Unique Identifier

### Example

```typescript
import {
    CustodianApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let id: string; //Custodian Unique Identifier (default to undefined)

const { status, data } = await apiInstance.custodianShowByUniqueIdentifier(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] | Custodian Unique Identifier | defaults to undefined|


### Return type

**CustodianIndex200Response**

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

# **custodianStore**
> CustodianStore201Response custodianStore(custodianStoreRequest)

Create a Custodian entry

### Example

```typescript
import {
    CustodianApi,
    Configuration,
    CustodianStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let custodianStoreRequest: CustodianStoreRequest; //Custodian definition

const { status, data } = await apiInstance.custodianStore(
    custodianStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianStoreRequest** | **CustodianStoreRequest**| Custodian definition | |


### Return type

**CustodianStore201Response**

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

# **custodianUpdate**
> CustodianStore201Response custodianUpdate(custodianStoreRequest)

Edit a Custodian entry

### Example

```typescript
import {
    CustodianApi,
    Configuration,
    CustodianStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianApi(configuration);

let id: number; //Custodian ID (default to undefined)
let custodianStoreRequest: CustodianStoreRequest; //Custodian definition

const { status, data } = await apiInstance.custodianUpdate(
    id,
    custodianStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianStoreRequest** | **CustodianStoreRequest**| Custodian definition | |
| **id** | [**number**] | Custodian ID | defaults to undefined|


### Return type

**CustodianStore201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

