# FeatureApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**featureIndex**](#featureindex) | **GET** /api/v1/features | Feature@index|
|[**featureShow**](#featureshow) | **GET** /api/v1/features/{featureId} | Feature@show|
|[**featureToggleByFeatureId**](#featuretogglebyfeatureid) | **PUT** /api/v1/features/{featureId}/toggle | Feature@show|

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

# **featureShow**
> FeatureIndex200Response featureShow()

Return a Feature entry by its ID

### Example

```typescript
import {
    FeatureApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new FeatureApi(configuration);

let featureId: number; //ID of the feature (default to undefined)

const { status, data } = await apiInstance.featureShow(
    featureId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **featureId** | [**number**] | ID of the feature | defaults to undefined|


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
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **featureToggleByFeatureId**
> FeatureIndex200Response featureToggleByFeatureId()

Toggle and return a Feature entry by its ID

### Example

```typescript
import {
    FeatureApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new FeatureApi(configuration);

let featureId: number; //ID of the feature (default to undefined)

const { status, data } = await apiInstance.featureToggleByFeatureId(
    featureId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **featureId** | [**number**] | ID of the feature | defaults to undefined|


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
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

