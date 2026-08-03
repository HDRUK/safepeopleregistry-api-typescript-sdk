# ValidationLogWithCommentsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**validationLogWithCommentsIndex**](#validationlogwithcommentsindex) | **GET** /api/v1/validation_logs/{id} | Get  a Validation Log|

# **validationLogWithCommentsIndex**
> Array<ValidationLog> validationLogWithCommentsIndex()

Retrieve a specific entry for a validation log .

### Example

```typescript
import {
    ValidationLogWithCommentsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogWithCommentsApi(configuration);

let id: number; //The ID of the validation log (default to undefined)

const { status, data } = await apiInstance.validationLogWithCommentsIndex(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | The ID of the validation log | defaults to undefined|


### Return type

**Array<ValidationLog>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation log with comments |  -  |
|**404** | Validation log not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

