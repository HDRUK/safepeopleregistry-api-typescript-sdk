# TrainingApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**trainingIndex**](#trainingindex) | **GET** /api/v1/training | Training@index|
|[**trainingIndexByRegistryId**](#trainingindexbyregistryid) | **GET** /api/v1/training/registry/{id} | Training@show|
|[**trainingShow**](#trainingshow) | **GET** /api/v1/training/{id} | Training@show|
|[**trainingStore**](#trainingstore) | **POST** /api/v1/training | Training@store|
|[**trainingUpdate**](#trainingupdate) | **PUT** /api/v1/training/{id} | Training@update|

# **trainingIndex**
> TrainingShow200Response trainingIndex()

Return a list of Training entries

### Example

```typescript
import {
    TrainingApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new TrainingApi(configuration);

const { status, data } = await apiInstance.trainingIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**TrainingShow200Response**

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

# **trainingIndexByRegistryId**
> TrainingShow200Response trainingIndexByRegistryId()

Return a list of training by registry id

### Example

```typescript
import {
    TrainingApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new TrainingApi(configuration);

let id: number; //Training registry id (default to undefined)

const { status, data } = await apiInstance.trainingIndexByRegistryId(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Training registry id | defaults to undefined|


### Return type

**TrainingShow200Response**

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

# **trainingShow**
> TrainingShow200Response trainingShow()

Return a training record by registry id

### Example

```typescript
import {
    TrainingApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new TrainingApi(configuration);

let id: number; //Training id (default to undefined)

const { status, data } = await apiInstance.trainingShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Training id | defaults to undefined|


### Return type

**TrainingShow200Response**

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

# **trainingStore**
> AccreditationStoreByRegistryId201Response trainingStore(training)

Create a Training entry

### Example

```typescript
import {
    TrainingApi,
    Configuration,
    Training
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new TrainingApi(configuration);

let training: Training; //Training definition

const { status, data } = await apiInstance.trainingStore(
    training
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **training** | **Training**| Training definition | |


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

# **trainingUpdate**
> TrainingUpdate200Response trainingUpdate(training)

Update a Training entry

### Example

```typescript
import {
    TrainingApi,
    Configuration,
    Training
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new TrainingApi(configuration);

let id: number; //Training entry ID (default to undefined)
let training: Training; //Training definition

const { status, data } = await apiInstance.trainingUpdate(
    id,
    training
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **training** | **Training**| Training definition | |
| **id** | [**number**] | Training entry ID | defaults to undefined|


### Return type

**TrainingUpdate200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

