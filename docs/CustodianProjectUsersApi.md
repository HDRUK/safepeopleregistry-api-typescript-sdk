# CustodianProjectUsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianProjectUsersIndex**](#custodianprojectusersindex) | **GET** /api/v1/custodian_approvals/{custodianId}/projectUsers | List all project users associated with a custodian|
|[**custodianProjectUsersShow**](#custodianprojectusersshow) | **GET** /api/v1/custodian_approvals/{custodianId}/projectUsers/{projectUserId} | Get custodian approval for a project user|
|[**custodianProjectUsersUpdate**](#custodianprojectusersupdate) | **PUT** /api/v1/custodian_approvals/{custodianId}/projectUsers/{projectUserId} | Update custodian approval for a project user|

# **custodianProjectUsersIndex**
> CustodianProjectUsersIndex200Response custodianProjectUsersIndex()

Returns a list of all custodian project user approvals for a specific custodian

### Example

```typescript
import {
    CustodianProjectUsersApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianProjectUsersApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)

const { status, data } = await apiInstance.custodianProjectUsersIndex(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**CustodianProjectUsersIndex200Response**

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

# **custodianProjectUsersShow**
> CustodianProjectUsersShow200Response custodianProjectUsersShow()

Returns custodian approval details for a specific project user

### Example

```typescript
import {
    CustodianProjectUsersApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianProjectUsersApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let projectUserId: number; //ID of the project user (default to undefined)

const { status, data } = await apiInstance.custodianProjectUsersShow(
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

**CustodianProjectUsersShow200Response**

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

# **custodianProjectUsersUpdate**
> CustodianProjectUsersShow200Response custodianProjectUsersUpdate(custodianProjectUsersUpdateRequest)

Updates approval status and/or comment for a project user

### Example

```typescript
import {
    CustodianProjectUsersApi,
    Configuration,
    CustodianProjectUsersUpdateRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianProjectUsersApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let projectUserId: number; //ID of the project user (default to undefined)
let custodianProjectUsersUpdateRequest: CustodianProjectUsersUpdateRequest; //

const { status, data } = await apiInstance.custodianProjectUsersUpdate(
    custodianId,
    projectUserId,
    custodianProjectUsersUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianProjectUsersUpdateRequest** | **CustodianProjectUsersUpdateRequest**|  | |
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|
| **projectUserId** | [**number**] | ID of the project user | defaults to undefined|


### Return type

**CustodianProjectUsersShow200Response**

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

