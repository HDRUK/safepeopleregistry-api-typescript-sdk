# CustodianUserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianUserBulkStore**](#custodianuserbulkstore) | **POST** /api/v1/custodian_users/bulk | Create multiple CustodianUser entries|

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

