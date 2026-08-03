# OrganisationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianProjectOrganisationsGetStatus**](#custodianprojectorganisationsgetstatus) | **GET** /api/v1/custodian_approvals/{custodianId}/project/{projectId}/organisation/{organisationId}/projectOrganisations/status | Get project organisation status|
|[**organisationsCustodianInviteUser**](#organisationscustodianinviteuser) | **POST** /api/v1/organisations/{id}/custodian_invite_user | organisations@custodian_invite_user|
|[**organisationsDestroy**](#organisationsdestroy) | **DELETE** /api/v1/organisations/{id} | organisations@destroy|
|[**organisationsGetRegistries**](#organisationsgetregistries) | **GET** /api/v1/organisations/{id}/registries | Get all registries for an organisation|
|[**organisationsGetStatus**](#organisationsgetstatus) | **GET** /api/v1/organisations/{id}/status | Get organisation status|
|[**organisationsIdvt**](#organisationsidvt) | **GET** /api/v1/organisations/{id}/idvt | organisations@idvt|
|[**organisationsInviteUser**](#organisationsinviteuser) | **POST** /api/v1/organisations/{id}/invite_user | organisations@invite_user|
|[**organisationsShow**](#organisationsshow) | **GET** /api/v1/organisations/{id} | organisations@show|
|[**organisationsStore**](#organisationsstore) | **POST** /api/v1/organisations | organisations@store|
|[**organisationsUpdate**](#organisationsupdate) | **PUT** /api/v1/organisations/{id} | organisations@update|
|[**organisationsUpdateApproved**](#organisationsupdateapproved) | **PUT** /api/v1/organisations/{id}/approved | SuperAdmin update org system_approved flag|

# **custodianProjectOrganisationsGetStatus**
> CustodianProjectOrganisationsGetStatus200Response custodianProjectOrganisationsGetStatus()

Retrieve the status of a project organisation for a specific custodian using custodianId, projectId, and organisationId.

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let custodianId: number; //Custodian ID (default to undefined)
let projectId: number; //Project ID (default to undefined)
let organisationId: number; //Organisation ID (default to undefined)

const { status, data } = await apiInstance.custodianProjectOrganisationsGetStatus(
    custodianId,
    projectId,
    organisationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | Custodian ID | defaults to undefined|
| **projectId** | [**number**] | Project ID | defaults to undefined|
| **organisationId** | [**number**] | Organisation ID | defaults to undefined|


### Return type

**CustodianProjectOrganisationsGetStatus200Response**

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
|**404** | Organisation or custodian project organisation not found |  -  |
|**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsCustodianInviteUser**
> AccreditationStoreByRegistryId201Response organisationsCustodianInviteUser(organisationsInviteUserRequest)

Invites a user to org

### Example

```typescript
import {
    OrganisationsApi,
    Configuration,
    OrganisationsInviteUserRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)
let organisationsInviteUserRequest: OrganisationsInviteUserRequest; //Invite definition

const { status, data } = await apiInstance.organisationsCustodianInviteUser(
    id,
    organisationsInviteUserRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationsInviteUserRequest** | **OrganisationsInviteUserRequest**| Invite definition | |
| **id** | [**number**] | organisations entry ID | defaults to undefined|


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
|**201** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsDestroy**
> AffiliationDestroy200Response organisationsDestroy()

Delete an organisations entry from the system

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)

const { status, data } = await apiInstance.organisationsDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | organisations entry ID | defaults to undefined|


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

# **organisationsGetRegistries**
> OrganisationsGetRegistries200Response organisationsGetRegistries()

Returns all registries associated with the specified organisation

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //Organisation ID (default to undefined)
let showPending: boolean; //Include users with pending invitations (true/false) (optional) (default to undefined)

const { status, data } = await apiInstance.organisationsGetRegistries(
    id,
    showPending
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Organisation ID | defaults to undefined|
| **showPending** | [**boolean**] | Include users with pending invitations (true/false) | (optional) defaults to undefined|


### Return type

**OrganisationsGetRegistries200Response**

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
|**404** | No registries found for this organisation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsGetStatus**
> CustodianProjectOrganisationsGetStatus200Response organisationsGetStatus()

Returns the organisation with its model state and state

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //Organisation ID (default to undefined)

const { status, data } = await apiInstance.organisationsGetStatus(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Organisation ID | defaults to undefined|


### Return type

**CustodianProjectOrganisationsGetStatus200Response**

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
|**404** | Organisation not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsIdvt**
> OrganisationsIdvt200Response organisationsIdvt()

Return an organisations idvt details by ID

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)

const { status, data } = await apiInstance.organisationsIdvt(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | organisations entry ID | defaults to undefined|


### Return type

**OrganisationsIdvt200Response**

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

# **organisationsInviteUser**
> AccreditationStoreByRegistryId201Response organisationsInviteUser(organisationsInviteUserRequest)

Invites a user to org

### Example

```typescript
import {
    OrganisationsApi,
    Configuration,
    OrganisationsInviteUserRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)
let organisationsInviteUserRequest: OrganisationsInviteUserRequest; //Invite definition

const { status, data } = await apiInstance.organisationsInviteUser(
    id,
    organisationsInviteUserRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationsInviteUserRequest** | **OrganisationsInviteUserRequest**| Invite definition | |
| **id** | [**number**] | organisations entry ID | defaults to undefined|


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
|**201** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**403** | forbidden |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsShow**
> OrganisationIndex200Response organisationsShow()

Return an organisations entry by ID

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)

const { status, data } = await apiInstance.organisationsShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | organisations entry ID | defaults to undefined|


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
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsStore**
> IdentityStore201Response organisationsStore(organisation)

Create a organisations entry

### Example

```typescript
import {
    OrganisationsApi,
    Configuration,
    Organisation
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let organisation: Organisation; //organisations definition

const { status, data } = await apiInstance.organisationsStore(
    organisation
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisation** | **Organisation**| organisations definition | |


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

# **organisationsUpdate**
> OrganisationsUpdate200Response organisationsUpdate(organisation)

Update a organisations entry

### Example

```typescript
import {
    OrganisationsApi,
    Configuration,
    Organisation
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)
let organisation: Organisation; //organisations definition

const { status, data } = await apiInstance.organisationsUpdate(
    id,
    organisation
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisation** | **Organisation**| organisations definition | |
| **id** | [**number**] | organisations entry ID | defaults to undefined|


### Return type

**OrganisationsUpdate200Response**

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

# **organisationsUpdateApproved**
> AccreditationStoreByRegistryId201Response organisationsUpdateApproved(organisationsUpdateApprovedRequest)

Updates the system_approved flag for an organisation

### Example

```typescript
import {
    OrganisationsApi,
    Configuration,
    OrganisationsUpdateApprovedRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)
let organisationsUpdateApprovedRequest: OrganisationsUpdateApprovedRequest; //System approval update definition

const { status, data } = await apiInstance.organisationsUpdateApproved(
    id,
    organisationsUpdateApprovedRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationsUpdateApprovedRequest** | **OrganisationsUpdateApprovedRequest**| System approval update definition | |
| **id** | [**number**] | organisations entry ID | defaults to undefined|


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
|**201** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

