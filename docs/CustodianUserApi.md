# CustodianUserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianUserBulkStore**](#custodianuserbulkstore) | **POST** /api/v1/custodian_users/bulk | Create multiple CustodianUser entries|
|[**custodianUserDestroy**](#custodianuserdestroy) | **DELETE** /api/v1/custodian_users/{id} | CustodianUser@destroy|
|[**custodianUserShow**](#custodianusershow) | **GET** /api/v1/custodian_users/{id} | CustodianUser@show|
|[**custodianUserStore**](#custodianuserstore) | **POST** /api/v1/custodian_users | CustodianUser@store|
|[**custodianUserUpdate**](#custodianuserupdate) | **PUT** /api/v1/custodian_users | CustodianUser@update|

# **custodianUserBulkStore**
> CustodianUserBulkStore201Response custodianUserBulkStore(custodianUserBulkStoreRequest)

Create multiple CustodianUser entries

### Example

```typescript
import {
    CustodianUserApi,
    Configuration,
    CustodianUserBulkStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianUserApi(configuration);

let custodianUserBulkStoreRequest: CustodianUserBulkStoreRequest; //Array of CustodianUser definitions

const { status, data } = await apiInstance.custodianUserBulkStore(
    custodianUserBulkStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianUserBulkStoreRequest** | **CustodianUserBulkStoreRequest**| Array of CustodianUser definitions | |


### Return type

**CustodianUserBulkStore201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianUserDestroy**
> AffiliationDestroy200Response custodianUserDestroy()

Delete a CustodianUser entry from the system

### Example

```typescript
import {
    CustodianUserApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianUserApi(configuration);

let id: number; //CustodianUser entry ID (default to undefined)

const { status, data } = await apiInstance.custodianUserDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | CustodianUser entry ID | defaults to undefined|


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

# **custodianUserShow**
> CustodianUserShow200Response custodianUserShow()

Return a CustodianUser entry by ID

### Example

```typescript
import {
    CustodianUserApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianUserApi(configuration);

let id: number; //CustodianUser entry ID (default to undefined)

const { status, data } = await apiInstance.custodianUserShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | CustodianUser entry ID | defaults to undefined|


### Return type

**CustodianUserShow200Response**

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

# **custodianUserStore**
> AccreditationStoreByRegistryId201Response custodianUserStore(custodianUser)

Create a CustodianUser entry

### Example

```typescript
import {
    CustodianUserApi,
    Configuration,
    CustodianUser
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianUserApi(configuration);

let custodianUser: CustodianUser; //CustodianUser definition

const { status, data } = await apiInstance.custodianUserStore(
    custodianUser
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianUser** | **CustodianUser**| CustodianUser definition | |


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
|**404** | Not found response |  -  |
|**201** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianUserUpdate**
> CustodianUserUpdate201Response custodianUserUpdate(custodianUser)

Update a CustodianUser entry

### Example

```typescript
import {
    CustodianUserApi,
    Configuration,
    CustodianUser
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianUserApi(configuration);

let custodianUser: CustodianUser; //CustodianUser definition

const { status, data } = await apiInstance.custodianUserUpdate(
    custodianUser
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianUser** | **CustodianUser**| CustodianUser definition | |


### Return type

**CustodianUserUpdate201Response**

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
|**400** | Invalid argument(s) |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

