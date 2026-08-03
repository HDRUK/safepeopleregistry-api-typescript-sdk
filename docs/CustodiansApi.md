# CustodiansApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodiansCreateCustodianValidationChecks**](#custodianscreatecustodianvalidationchecks) | **POST** /api/v1/custodians/{custodianId}/validation_checks | Assign a validation check to a custodian|
|[**custodiansGetCustodianUsers**](#custodiansgetcustodianusers) | **GET** /api/v1/custodians/{custodianId}/custodian_users | Get list of people for a custodian|
|[**custodiansGetCustodianValidationChecks**](#custodiansgetcustodianvalidationchecks) | **GET** /api/v1/custodians/{custodianId}/validation_checks | Get validation checks assigned to a custodian|
|[**custodiansGetOrganisationUsers**](#custodiansgetorganisationusers) | **GET** /api/v1/custodians/{custodianId}/organisations/{organisationId}/users | Get list of people for organisation|
|[**custodiansGetRules**](#custodiansgetrules) | **GET** /api/v1/custodians/{id}/rules | Get rules for a specific custodian|
|[**custodiansGetStatusesUsers**](#custodiansgetstatusesusers) | **GET** /api/v1/custodians/{custodianId}/projectUsers/{projectUserId}/statuses | Get statuses for a user in a project/organisation/custodian|

# **custodiansCreateCustodianValidationChecks**
> ValidationCheck custodiansCreateCustodianValidationChecks(custodiansCreateCustodianValidationChecksRequest)

Creates a new validation check and assigns it to a specific custodian via the custodian_has_validation_check pivot table.

### Example

```typescript
import {
    CustodiansApi,
    Configuration,
    CustodiansCreateCustodianValidationChecksRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodiansApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let custodiansCreateCustodianValidationChecksRequest: CustodiansCreateCustodianValidationChecksRequest; //

const { status, data } = await apiInstance.custodiansCreateCustodianValidationChecks(
    custodianId,
    custodiansCreateCustodianValidationChecksRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodiansCreateCustodianValidationChecksRequest** | **CustodiansCreateCustodianValidationChecksRequest**|  | |
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**ValidationCheck**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Validation check created and assigned successfully |  -  |
|**400** | Invalid input |  -  |
|**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodiansGetCustodianUsers**
> CustodiansGetCustodianUsers200Response custodiansGetCustodianUsers()

Fetches the list of custodian users based on the custodian id.

### Example

```typescript
import {
    CustodiansApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodiansApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)

const { status, data } = await apiInstance.custodiansGetCustodianUsers(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**CustodiansGetCustodianUsers200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successfully retrieved custodian users |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Custodian users not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodiansGetCustodianValidationChecks**
> Array<ValidationCheck> custodiansGetCustodianValidationChecks()

Returns the list of validation checks associated with a specific custodian.

### Example

```typescript
import {
    CustodiansApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodiansApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)

const { status, data } = await apiInstance.custodiansGetCustodianValidationChecks(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**Array<ValidationCheck>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation checks retrieved successfully |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodiansGetOrganisationUsers**
> CustodiansGetOrganisationUsers200Response custodiansGetOrganisationUsers()

Fetches the list of users associated with the given custodian and organisations IDs.

### Example

```typescript
import {
    CustodiansApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodiansApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let organisationId: number; //ID of the organisation (default to undefined)

const { status, data } = await apiInstance.custodiansGetOrganisationUsers(
    custodianId,
    organisationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|
| **organisationId** | [**number**] | ID of the organisation | defaults to undefined|


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

# **custodiansGetRules**
> CustodiansGetRules200Response custodiansGetRules()

Fetches the list of rules associated with the given custodian ID.

### Example

```typescript
import {
    CustodiansApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodiansApi(configuration);

let id: number; //ID of the custodian (default to undefined)

const { status, data } = await apiInstance.custodiansGetRules(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**CustodiansGetRules200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successfully retrieved rules |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodiansGetStatusesUsers**
> CustodiansGetOrganisationUsers200Response custodiansGetStatusesUsers()

Fetches the user statuses given custodian and organisations and project and user IDs.

### Example

```typescript
import {
    CustodiansApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodiansApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let projectUserId: number; //ID of the project user (default to undefined)

const { status, data } = await apiInstance.custodiansGetStatusesUsers(
    custodianId,
    projectUserId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|
| **projectUserId** | [**number**] | ID of the project user | defaults to undefined|


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

