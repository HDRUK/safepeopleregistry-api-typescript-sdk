# EndorsementsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**endorsementsStore**](#endorsementsstore) | **POST** /api/v1/endorsements | Endorsements@store|

# **endorsementsStore**
> EndorsementsStore201Response endorsementsStore(endorsementsStoreRequest)

Create an Endorsements entry

### Example

```typescript
import {
    EndorsementsApi,
    Configuration,
    EndorsementsStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EndorsementsApi(configuration);

let endorsementsStoreRequest: EndorsementsStoreRequest; //Endorsements definition

const { status, data } = await apiInstance.endorsementsStore(
    endorsementsStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **endorsementsStoreRequest** | **EndorsementsStoreRequest**| Endorsements definition | |


### Return type

**EndorsementsStore201Response**

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

