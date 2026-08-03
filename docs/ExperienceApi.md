# ExperienceApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**experienceDestroy**](#experiencedestroy) | **DELETE** /api/v1/experiences/{id} | Experience@destroy|
|[**experienceIndex**](#experienceindex) | **GET** /api/v1/experiences | Experience@index|
|[**experienceShow**](#experienceshow) | **GET** /api/v1/experiences/{id} | Experience@show|
|[**experienceStore**](#experiencestore) | **POST** /api/v1/experiences | Experience@store|
|[**experienceUpdate**](#experienceupdate) | **PUT** /api/v1/experiences/{id} | Experience@update|

# **experienceDestroy**
> AffiliationDestroy200Response experienceDestroy()

Delete a Experience entry from the system

### Example

```typescript
import {
    ExperienceApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ExperienceApi(configuration);

let id: number; //Experience entry ID (default to undefined)

const { status, data } = await apiInstance.experienceDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Experience entry ID | defaults to undefined|


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

# **experienceIndex**
> ExperienceIndex200Response experienceIndex()

Return a list of Experience entries

### Example

```typescript
import {
    ExperienceApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ExperienceApi(configuration);

const { status, data } = await apiInstance.experienceIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**ExperienceIndex200Response**

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

# **experienceShow**
> ExperienceShow200Response experienceShow()

Return an Experience entry by ID

### Example

```typescript
import {
    ExperienceApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ExperienceApi(configuration);

let id: number; //Experience entry ID (default to undefined)

const { status, data } = await apiInstance.experienceShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | Experience entry ID | defaults to undefined|


### Return type

**ExperienceShow200Response**

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

# **experienceStore**
> ExperienceStore201Response experienceStore(experienceStoreRequest)

Create an Experience entry

### Example

```typescript
import {
    ExperienceApi,
    Configuration,
    ExperienceStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ExperienceApi(configuration);

let experienceStoreRequest: ExperienceStoreRequest; //Experience definition

const { status, data } = await apiInstance.experienceStore(
    experienceStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **experienceStoreRequest** | **ExperienceStoreRequest**| Experience definition | |


### Return type

**ExperienceStore201Response**

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

# **experienceUpdate**
> ExperienceUpdate200Response experienceUpdate(experienceStoreRequest)

Update an Experience entry

### Example

```typescript
import {
    ExperienceApi,
    Configuration,
    ExperienceStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ExperienceApi(configuration);

let id: number; //Experience entry ID (default to undefined)
let experienceStoreRequest: ExperienceStoreRequest; //Experience definition

const { status, data } = await apiInstance.experienceUpdate(
    id,
    experienceStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **experienceStoreRequest** | **ExperienceStoreRequest**| Experience definition | |
| **id** | [**number**] | Experience entry ID | defaults to undefined|


### Return type

**ExperienceUpdate200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

