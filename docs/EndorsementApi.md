# EndorsementApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**endorsementIndex**](#endorsementindex) | **GET** /api/v1/endorsements | Endorsement@index|
|[**endorsementShow**](#endorsementshow) | **GET** /api/v1/endorsements/{id} | Endorsement@show|

# **endorsementIndex**
> EndorsementIndex200Response endorsementIndex()

Return a list of Endorsements

### Example

```typescript
import {
    EndorsementApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EndorsementApi(configuration);

const { status, data } = await apiInstance.endorsementIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**EndorsementIndex200Response**

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

# **endorsementShow**
> EndorsementIndex200Response endorsementShow()

Return an Endorsement entry by ID

### Example

```typescript
import {
    EndorsementApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new EndorsementApi(configuration);

let id: number; //Endorsement entry ID (default to undefined)

const { status, data } = await apiInstance.endorsementShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Endorsement entry ID | defaults to undefined|


### Return type

**EndorsementIndex200Response**

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

