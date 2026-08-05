# FeatureApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**featureIndex**](#featureindex) | **GET** /api/v1/features | Feature@index|

# **featureIndex**
> FeatureIndex200Response featureIndex()

Return a list of Feature entries

### Example

```typescript
import {
    FeatureApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new FeatureApi(configuration);

const { status, data } = await apiInstance.featureIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**FeatureIndex200Response**

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

