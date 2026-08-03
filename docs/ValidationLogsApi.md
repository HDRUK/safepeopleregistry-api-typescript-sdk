# ValidationLogsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**validationLogsGetCustodianOrganisationValidationLogs**](#validationlogsgetcustodianorganisationvalidationlogs) | **GET** /api/v1/custodians/{custodianId}/organisation/{organisationId}/validation_logs | Get Validation Logs for Custodian and Organisation|
|[**validationLogsGetCustodianProjectUserValidationLogs**](#validationlogsgetcustodianprojectuservalidationlogs) | **GET** /api/v1/custodians/{custodianId}/projects/{projectId}/registries/{registryId}/validation_logs | Get Validation Logs for Custodian, Project, and Registry|
|[**validationLogsUpdate**](#validationlogsupdate) | **PUT** /api/v1/validation_logs/{id} | Update a Validation Log|
|[**validationLogsUpdateCustodianValidationLogs**](#validationlogsupdatecustodianvalidationlogs) | **PUT** /api/v1/custodians/{custodianId}/validation_Logs | Enable or Disable All Validation Logs for a Custodian Across Projects/Registries|

# **validationLogsGetCustodianOrganisationValidationLogs**
> ValidationLogsGetCustodianProjectUserValidationLogs200Response validationLogsGetCustodianOrganisationValidationLogs()

Retrieve validation logs associated with a given custodian and organisation.

### Example

```typescript
import {
    ValidationLogsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogsApi(configuration);

let custodianId: number; //The ID of the custodian entity (default to undefined)
let organisationId: number; //The ID of the organisation entity (default to undefined)
let showDisabled: boolean; //Whether to include disabled validation logs (optional) (default to undefined)

const { status, data } = await apiInstance.validationLogsGetCustodianOrganisationValidationLogs(
    custodianId,
    organisationId,
    showDisabled
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | The ID of the custodian entity | defaults to undefined|
| **organisationId** | [**number**] | The ID of the organisation entity | defaults to undefined|
| **showDisabled** | [**boolean**] | Whether to include disabled validation logs | (optional) defaults to undefined|


### Return type

**ValidationLogsGetCustodianProjectUserValidationLogs200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response with validation logs |  -  |
|**404** | Custodian or Organisation not found |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationLogsGetCustodianProjectUserValidationLogs**
> ValidationLogsGetCustodianProjectUserValidationLogs200Response validationLogsGetCustodianProjectUserValidationLogs()

Retrieve validation logs associated with a given custodian, project, and registry.

### Example

```typescript
import {
    ValidationLogsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogsApi(configuration);

let custodianId: number; //The ID of the custodian entity (default to undefined)
let projectId: number; //The ID of the project entity (default to undefined)
let registryId: number; //The ID of the registry entity (default to undefined)

const { status, data } = await apiInstance.validationLogsGetCustodianProjectUserValidationLogs(
    custodianId,
    projectId,
    registryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | The ID of the custodian entity | defaults to undefined|
| **projectId** | [**number**] | The ID of the project entity | defaults to undefined|
| **registryId** | [**number**] | The ID of the registry entity | defaults to undefined|


### Return type

**ValidationLogsGetCustodianProjectUserValidationLogs200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response with validation logs |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationLogsUpdate**
> ValidationLogsUpdate200Response validationLogsUpdate()

Update a validation log entry, including marking it as complete, incomplete, passed, or failed.

### Example

```typescript
import {
    ValidationLogsApi,
    Configuration,
    ValidationLogsUpdateRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogsApi(configuration);

let id: number; //The ID of the validation log entry (default to undefined)
let validationLogsUpdateRequest: ValidationLogsUpdateRequest; // (optional)

const { status, data } = await apiInstance.validationLogsUpdate(
    id,
    validationLogsUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **validationLogsUpdateRequest** | **ValidationLogsUpdateRequest**|  | |
| **id** | [**number**] | The ID of the validation log entry | defaults to undefined|


### Return type

**ValidationLogsUpdate200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation log status updated successfully |  -  |
|**404** | Validation log not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationLogsUpdateCustodianValidationLogs**
> ValidationLogsUpdateCustodianValidationLogs200Response validationLogsUpdateCustodianValidationLogs(validationLogsUpdateCustodianValidationLogsRequest)

Bulk update the enabled flag for all validation logs tied to a custodian and any project/registry.

### Example

```typescript
import {
    ValidationLogsApi,
    Configuration,
    ValidationLogsUpdateCustodianValidationLogsRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogsApi(configuration);

let custodianId: number; //The ID of the custodian entity (default to undefined)
let validationLogsUpdateCustodianValidationLogsRequest: ValidationLogsUpdateCustodianValidationLogsRequest; //

const { status, data } = await apiInstance.validationLogsUpdateCustodianValidationLogs(
    custodianId,
    validationLogsUpdateCustodianValidationLogsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **validationLogsUpdateCustodianValidationLogsRequest** | **ValidationLogsUpdateCustodianValidationLogsRequest**|  | |
| **custodianId** | [**number**] | The ID of the custodian entity | defaults to undefined|


### Return type

**ValidationLogsUpdateCustodianValidationLogs200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation logs updated successfully |  -  |
|**400** | Invalid request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

