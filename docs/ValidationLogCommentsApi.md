# ValidationLogCommentsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**validationLogCommentsComments**](#validationlogcommentscomments) | **GET** /api/v1/validation_logs/{id}/comments | Get all comments for a Validation Log|
|[**validationLogCommentsDestroy**](#validationlogcommentsdestroy) | **DELETE** /api/v1/validation_log_comments/{id} | Delete a validation log comment|
|[**validationLogCommentsShow**](#validationlogcommentsshow) | **GET** /api/v1/validation_log_comments/{id} | Get a single validation log comment|
|[**validationLogCommentsStore**](#validationlogcommentsstore) | **POST** /api/v1/validation_log_comments | Create a new validation log comment|
|[**validationLogCommentsUpdate**](#validationlogcommentsupdate) | **PUT** /api/v1/validation_log_comments/{id} | Update a validation log comment|

# **validationLogCommentsComments**
> Array<ValidationLog> validationLogCommentsComments()

Retrieve all comments associated with a specific validation log entry.

### Example

```typescript
import {
    ValidationLogCommentsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogCommentsApi(configuration);

let id: number; //The ID of the validation log (default to undefined)

const { status, data } = await apiInstance.validationLogCommentsComments(
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

# **validationLogCommentsDestroy**
> ValidationLogCommentsDestroy200Response validationLogCommentsDestroy()

Remove a comment from the validation logs.

### Example

```typescript
import {
    ValidationLogCommentsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogCommentsApi(configuration);

let id: number; //The ID of the comment (default to undefined)

const { status, data } = await apiInstance.validationLogCommentsDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | The ID of the comment | defaults to undefined|


### Return type

**ValidationLogCommentsDestroy200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Comment deleted successfully |  -  |
|**400** | Comment not found |  -  |
|**404** | Comment not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationLogCommentsShow**
> ValidationLogComment validationLogCommentsShow()

Retrieve a specific validation log comment by ID.

### Example

```typescript
import {
    ValidationLogCommentsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogCommentsApi(configuration);

let id: number; //The ID of the comment (default to undefined)

const { status, data } = await apiInstance.validationLogCommentsShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | The ID of the comment | defaults to undefined|


### Return type

**ValidationLogComment**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Comment retrieved successfully |  -  |
|**400** | Comment not found |  -  |
|**404** | Comment not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationLogCommentsStore**
> ValidationLogComment validationLogCommentsStore(validationLogCommentsStoreRequest)

Add a new comment to a validation log.

### Example

```typescript
import {
    ValidationLogCommentsApi,
    Configuration,
    ValidationLogCommentsStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogCommentsApi(configuration);

let validationLogCommentsStoreRequest: ValidationLogCommentsStoreRequest; //

const { status, data } = await apiInstance.validationLogCommentsStore(
    validationLogCommentsStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **validationLogCommentsStoreRequest** | **ValidationLogCommentsStoreRequest**|  | |


### Return type

**ValidationLogComment**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Comment created successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationLogCommentsUpdate**
> ValidationLogComment validationLogCommentsUpdate(validationLogCommentsUpdateRequest)

Edit an existing validation log comment.

### Example

```typescript
import {
    ValidationLogCommentsApi,
    Configuration,
    ValidationLogCommentsUpdateRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationLogCommentsApi(configuration);

let id: number; //The ID of the comment (default to undefined)
let validationLogCommentsUpdateRequest: ValidationLogCommentsUpdateRequest; //

const { status, data } = await apiInstance.validationLogCommentsUpdate(
    id,
    validationLogCommentsUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **validationLogCommentsUpdateRequest** | **ValidationLogCommentsUpdateRequest**|  | |
| **id** | [**number**] | The ID of the comment | defaults to undefined|


### Return type

**ValidationLogComment**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Comment updated successfully |  -  |
|**400** | Comment not found |  -  |
|**404** | Comment not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

