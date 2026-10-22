# OrganisationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**organisationsAppointSro**](#organisationsappointsro) | **PUT** /api/v1/organisations/{id}/sro | organisations@appointSro|
|[**organisationsInviteSro**](#organisationsinvitesro) | **POST** /api/v1/organisations/{id}/sro/invite | organisations@inviteSro|
|[**organisationsRemoveDelegate**](#organisationsremovedelegate) | **DELETE** /api/v1/organisations/{id}/delegates/{userId} | organisations@removeDelegate|
|[**organisationsResendSroInvite**](#organisationsresendsroinvite) | **POST** /api/v1/organisations/{id}/sro/resend_invite | organisations@resendSroInvite|

# **organisationsAppointSro**
> OrganisationsAppointSro200Response organisationsAppointSro(organisationsAppointSroRequest)

Hands the SRO role over immediately: the appointee becomes SRO, the current SRO becomes a delegate, and an invited SRO keeps their invitation but will join as a delegate. Delegates can appoint while the organisation has no claimed SRO; after that only the SRO can.

### Example

```typescript
import {
    OrganisationsApi,
    Configuration,
    OrganisationsAppointSroRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)
let organisationsAppointSroRequest: OrganisationsAppointSroRequest; //

const { status, data } = await apiInstance.organisationsAppointSro(
    id,
    organisationsAppointSroRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationsAppointSroRequest** | **OrganisationsAppointSroRequest**|  | |
| **id** | [**number**] | organisations entry ID | defaults to undefined|


### Return type

**OrganisationsAppointSro200Response**

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
|**403** | Forbidden |  -  |
|**404** | The user is not a claimed member of this organisation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsInviteSro**
> OrganisationsInviteSro201Response organisationsInviteSro(organisationsInviteSroRequest)

Creates an invited (unclaimed) SRO and emails them an invitation. The current SRO keeps the role until the invitee claims their account; any other invited SRO keeps their invitation but will join as a delegate. Delegates can invite while the organisation has no claimed SRO; after that only the SRO can.

### Example

```typescript
import {
    OrganisationsApi,
    Configuration,
    OrganisationsInviteSroRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)
let organisationsInviteSroRequest: OrganisationsInviteSroRequest; //

const { status, data } = await apiInstance.organisationsInviteSro(
    id,
    organisationsInviteSroRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationsInviteSroRequest** | **OrganisationsInviteSroRequest**|  | |
| **id** | [**number**] | organisations entry ID | defaults to undefined|


### Return type

**OrganisationsInviteSro201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Created |  -  |
|**400** | Invalid argument(s) |  -  |
|**403** | Forbidden |  -  |
|**409** | The email already belongs to a user; appoint an existing member with PUT /organisations/{id}/sro instead |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsRemoveDelegate**
> OrganisationsAppointSro200Response organisationsRemoveDelegate()

Detaches a delegate from the organisation and notifies them and the remaining members. The SRO and delegates of the organisation can remove other delegates; the SRO cannot be removed and nobody can remove themselves.

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)
let userId: number; //ID of the delegate to remove (default to undefined)

const { status, data } = await apiInstance.organisationsRemoveDelegate(
    id,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | organisations entry ID | defaults to undefined|
| **userId** | [**number**] | ID of the delegate to remove | defaults to undefined|


### Return type

**OrganisationsAppointSro200Response**

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
|**404** | The user is not a delegate of this organisation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisationsResendSroInvite**
> OrganisationsAppointSro200Response organisationsResendSroInvite()

Resends the pending SRO invitation with the code it already has. Delegates can resend while the organisation has no claimed SRO; after that only the SRO can.

### Example

```typescript
import {
    OrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new OrganisationsApi(configuration);

let id: number; //organisations entry ID (default to undefined)

const { status, data } = await apiInstance.organisationsResendSroInvite(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | organisations entry ID | defaults to undefined|


### Return type

**OrganisationsAppointSro200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**403** | Forbidden |  -  |
|**404** | The organisation has no pending SRO invitation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

