# QueryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**queryQuery**](#queryquery) | **POST** /api/v1/query | Query@query|

# **queryQuery**
> QueryQuery200Response queryQuery(queryQueryRequest)

Query the registry by Digital Identifier

### Example

```typescript
import {
    QueryApi,
    Configuration,
    QueryQueryRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new QueryApi(configuration);

let xClientId: string; //Custodian client ID used to authenticate the requesting custodian (default to undefined)
let queryQueryRequest: QueryQueryRequest; //Query definition

const { status, data } = await apiInstance.queryQuery(
    xClientId,
    queryQueryRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **queryQueryRequest** | **QueryQueryRequest**| Query definition | |
| **xClientId** | [**string**] | Custodian client ID used to authenticate the requesting custodian | defaults to undefined|


### Return type

**QueryQuery200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**401** | Unauthorised - missing or unrecognised x-client-id header |  -  |
|**404** | Not found response |  -  |
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

