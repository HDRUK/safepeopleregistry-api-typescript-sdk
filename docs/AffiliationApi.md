# AffiliationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**affiliationDestroy**](#affiliationdestroy) | **DELETE** /api/v1/training/{id} | Affiliation@destroy|

# **affiliationDestroy**
> AffiliationDestroy200Response affiliationDestroy()

Delete a affiliation entry from the system

### Example

```typescript
import {
    AffiliationApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new AffiliationApi(configuration);

let id: number; //Affiliation entry ID (default to undefined)

const { status, data } = await apiInstance.affiliationDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Affiliation entry ID | defaults to undefined|


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

