# OrganisationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**organisationGetDelegates**](#organisationgetdelegates) | **GET** /api/v1/organisations/{id}/delegates | Return all delegates associated with an organisation|
|[**organisationGetProjects**](#organisationgetprojects) | **GET** /api/v1/organisations/{id}/projects | organisation@getProjects|
|[**organisationGetSponsorshipsProjects**](#organisationgetsponsorshipsprojects) | **GET** /api/v1/organisations/{id}/projects/sponsorships | organisation@getSponsorshipsProjects|
|[**organisationGetUsers**](#organisationgetusers) | **GET** /api/v1/organisations/{id}/users | organisation@getUsers|
|[**organisationIndex**](#organisationindex) | **GET** /api/v1/organisations | organisation@index|

# **organisationGetDelegates**
> OrganisationGetDelegates200Response organisationGetDelegates()

Return all delegates associated with an organisation

### Example

```typescript
import {
    OrganisationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationApi(configuration);

let id: number; //Organisation ID (default to undefined)

const { status, data } = await apiInstance.organisationGetDelegates(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Organisation ID | defaults to undefined|


### Return type

**OrganisationGetDelegates200Response**

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

# **organisationGetProjects**
> OrganisationGetProjects200Response organisationGetProjects()

Return an all projects associated with an organisation (i.e. data-custodian)

### Example

```typescript
import {
    OrganisationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationApi(configuration);

let id: number; //Organisation ID (default to undefined)

const { status, data } = await apiInstance.organisationGetProjects(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Organisation ID | defaults to undefined|


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

# **organisationGetSponsorshipsProjects**
> OrganisationGetProjects200Response organisationGetSponsorshipsProjects()

Return an all projects associated with an organisation with sponsorships (i.e. data-custodian)

### Example

```typescript
import {
    OrganisationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationApi(configuration);

let id: number; //Organisation ID (default to undefined)

const { status, data } = await apiInstance.organisationGetSponsorshipsProjects(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Organisation ID | defaults to undefined|


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

# **organisationGetUsers**
> OrganisationGetUsers200Response organisationGetUsers()

Return all users associated with an organisation

### Example

```typescript
import {
    OrganisationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationApi(configuration);

let id: number; //Organisation ID (default to undefined)

const { status, data } = await apiInstance.organisationGetUsers(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Organisation ID | defaults to undefined|


### Return type

**OrganisationGetUsers200Response**

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

# **organisationIndex**
> OrganisationIndex200Response organisationIndex()

Return a list of organisations

### Example

```typescript
import {
    OrganisationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationApi(configuration);

const { status, data } = await apiInstance.organisationIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**OrganisationIndex200Response**

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

