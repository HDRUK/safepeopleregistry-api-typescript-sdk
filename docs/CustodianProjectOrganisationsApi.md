# CustodianProjectOrganisationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianProjectOrganisationsGetWorkflowStates**](#custodianprojectorganisationsgetworkflowstates) | **GET** /api/v1/custodian_approvals/projectOrganisations/getWorkflowStates | Get all workflow states for custodian project organisation approvals|
|[**custodianProjectOrganisationsIndex**](#custodianprojectorganisationsindex) | **GET** /api/v1/custodian_approvals/{custodianId}/projectOrganisations | List all project organisations associated with a custodian|
|[**custodianProjectOrganisationsShow**](#custodianprojectorganisationsshow) | **GET** /api/v1/custodian_approvals/{custodianId}/projectOrganisations/{projectOrganisationId} | Get custodian approval for a project organisation|
|[**custodianProjectOrganisationsUpdate**](#custodianprojectorganisationsupdate) | **PUT** /api/v1/custodian_approvals/{custodianId}/projectOrganisations/{projectOrganisationId} | Update custodian approval for a project organisation|

# **custodianProjectOrganisationsGetWorkflowStates**
> CustodianProjectOrganisationsGetWorkflowStates200Response custodianProjectOrganisationsGetWorkflowStates()

Returns a list of all possible workflow states

### Example

```typescript
import {
    CustodianProjectOrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianProjectOrganisationsApi(configuration);

const { status, data } = await apiInstance.custodianProjectOrganisationsGetWorkflowStates();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CustodianProjectOrganisationsGetWorkflowStates200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianProjectOrganisationsIndex**
> CustodianProjectOrganisationsIndex200Response custodianProjectOrganisationsIndex()

Returns a list of all custodian project organisation approvals for a specific custodian

### Example

```typescript
import {
    CustodianProjectOrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianProjectOrganisationsApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)

const { status, data } = await apiInstance.custodianProjectOrganisationsIndex(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**CustodianProjectOrganisationsIndex200Response**

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
|**403** | Forbidden |  -  |
|**404** | Custodian Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianProjectOrganisationsShow**
> CustodianProjectOrganisationsShow200Response custodianProjectOrganisationsShow()

Returns custodian approval details for a specific project organisation

### Example

```typescript
import {
    CustodianProjectOrganisationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianProjectOrganisationsApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let projectOrganisationId: number; //ID of the project organisation (default to undefined)

const { status, data } = await apiInstance.custodianProjectOrganisationsShow(
    custodianId,
    projectOrganisationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|
| **projectOrganisationId** | [**number**] | ID of the project organisation | defaults to undefined|


### Return type

**CustodianProjectOrganisationsShow200Response**

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
|**403** | Forbidden |  -  |
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianProjectOrganisationsUpdate**
> CustodianProjectOrganisationsShow200Response custodianProjectOrganisationsUpdate(custodianProjectOrganisationsUpdateRequest)

Updates approval status and/or comment for a project organisation

### Example

```typescript
import {
    CustodianProjectOrganisationsApi,
    Configuration,
    CustodianProjectOrganisationsUpdateRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianProjectOrganisationsApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let projectOrganisationId: number; //ID of the project organisation (default to undefined)
let custodianProjectOrganisationsUpdateRequest: CustodianProjectOrganisationsUpdateRequest; //

const { status, data } = await apiInstance.custodianProjectOrganisationsUpdate(
    custodianId,
    projectOrganisationId,
    custodianProjectOrganisationsUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianProjectOrganisationsUpdateRequest** | **CustodianProjectOrganisationsUpdateRequest**|  | |
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|
| **projectOrganisationId** | [**number**] | ID of the project organisation | defaults to undefined|


### Return type

**CustodianProjectOrganisationsShow200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |
|**400** | Invalid argument(s) |  -  |
|**403** | Forbidden |  -  |
|**404** | Not Found |  -  |
|**500** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

