# AffiliationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**affiliationsGetOrganisationAffiliation**](#affiliationsgetorganisationaffiliation) | **GET** /api/v1/affiliations/{registryId}/organisation/{organisationId} | Return a specific organisation\&#39;s affiliation by registry ID and organisation ID|
|[**affiliationsIndexByRegistryId**](#affiliationsindexbyregistryid) | **GET** /api/v1/affiliations/{registryId} | Affiliations@show|
|[**affiliationsStoreByRegistryId**](#affiliationsstorebyregistryid) | **POST** /api/v1/affiliations/{registryId} | Affiliations@store|
|[**affiliationsUpdate**](#affiliationsupdate) | **PUT** /api/v1/affiliations/{id} | Affiliations@update|
|[**affiliationsVerifyEmail**](#affiliationsverifyemail) | **PUT** /api/v1/affiliations/verify_email/{verificationCode} | Affiliations@verifyEmail|

# **affiliationsGetOrganisationAffiliation**
> AffiliationsGetOrganisationAffiliation200Response affiliationsGetOrganisationAffiliation()

Get a specific organisation\'s affiliation for a given registry

### Example

```typescript
import {
    AffiliationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AffiliationsApi(configuration);

let registryId: number; //Registry ID (default to undefined)
let organisationId: number; //Organisation ID (default to undefined)

const { status, data } = await apiInstance.affiliationsGetOrganisationAffiliation(
    registryId,
    organisationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | Registry ID | defaults to undefined|
| **organisationId** | [**number**] | Organisation ID | defaults to undefined|


### Return type

**AffiliationsGetOrganisationAffiliation200Response**

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
|**404** | Affiliation not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **affiliationsIndexByRegistryId**
> AffiliationsIndexByRegistryId200Response affiliationsIndexByRegistryId()

Return a list of affiliations by registry id

### Example

```typescript
import {
    AffiliationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AffiliationsApi(configuration);

let registryId: number; //Affiliations registry id (default to undefined)

const { status, data } = await apiInstance.affiliationsIndexByRegistryId(
    registryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registryId** | [**number**] | Affiliations registry id | defaults to undefined|


### Return type

**AffiliationsIndexByRegistryId200Response**

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

# **affiliationsStoreByRegistryId**
> AffiliationsStoreByRegistryId200Response affiliationsStoreByRegistryId(affiliation)

Create an Affiliation entry

### Example

```typescript
import {
    AffiliationsApi,
    Configuration,
    Affiliation
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AffiliationsApi(configuration);

let registryId: number; //Registry entry ID (default to undefined)
let affiliation: Affiliation; //Affiliation definition

const { status, data } = await apiInstance.affiliationsStoreByRegistryId(
    registryId,
    affiliation
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **affiliation** | **Affiliation**| Affiliation definition | |
| **registryId** | [**number**] | Registry entry ID | defaults to undefined|


### Return type

**AffiliationsStoreByRegistryId200Response**

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

# **affiliationsUpdate**
> AffiliationsStoreByRegistryId200Response affiliationsUpdate(affiliation)

Update an Affiliation entry

### Example

```typescript
import {
    AffiliationsApi,
    Configuration,
    Affiliation
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AffiliationsApi(configuration);

let id: number; //Affiliation entry ID (default to undefined)
let affiliation: Affiliation; //Affiliation definition

const { status, data } = await apiInstance.affiliationsUpdate(
    id,
    affiliation
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **affiliation** | **Affiliation**| Affiliation definition | |
| **id** | [**number**] | Affiliation entry ID | defaults to undefined|


### Return type

**AffiliationsStoreByRegistryId200Response**

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

# **affiliationsVerifyEmail**
> AffiliationsStoreByRegistryId200Response affiliationsVerifyEmail()

Update an Affiliation entry with verification

### Example

```typescript
import {
    AffiliationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AffiliationsApi(configuration);

let verificationCode: string; //Email verification code (default to undefined)

const { status, data } = await apiInstance.affiliationsVerifyEmail(
    verificationCode
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **verificationCode** | [**string**] | Email verification code | defaults to undefined|


### Return type

**AffiliationsStoreByRegistryId200Response**

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

