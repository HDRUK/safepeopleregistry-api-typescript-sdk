# HistoryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**historyIndex**](#historyindex) | **GET** /api/v1/histories | History@index|
|[**historyShow**](#historyshow) | **GET** /api/v1/histories/{id} | History@show|
|[**historyStore**](#historystore) | **POST** /api/v1/histories | History@store|

# **historyIndex**
> HistoryIndex200Response historyIndex()

Return a list of Histories

### Example

```typescript
import {
    HistoryApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new HistoryApi(configuration);

const { status, data } = await apiInstance.historyIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**HistoryIndex200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **historyShow**
> HistoryIndex200Response historyShow()

Return a History entry by ID

### Example

```typescript
import {
    HistoryApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new HistoryApi(configuration);

let id: number; //History entry ID (default to undefined)

const { status, data } = await apiInstance.historyShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | History entry ID | defaults to undefined|


### Return type

**HistoryIndex200Response**

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

# **historyStore**
> HistoryStore201Response historyStore(historyStoreRequest)

Create a History entry

### Example

```typescript
import {
    HistoryApi,
    Configuration,
    HistoryStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new HistoryApi(configuration);

let historyStoreRequest: HistoryStoreRequest; //History definition

const { status, data } = await apiInstance.historyStore(
    historyStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **historyStoreRequest** | **HistoryStoreRequest**| History definition | |


### Return type

**HistoryStore201Response**

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

