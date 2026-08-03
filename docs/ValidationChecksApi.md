# ValidationChecksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**validationChecksDestroy**](#validationchecksdestroy) | **DELETE** /api/v1/validation_checks/{id} | Delete a validation check|
|[**validationChecksIndex**](#validationchecksindex) | **GET** /api/v1/validation_checks | List all validation checks|
|[**validationChecksShow**](#validationchecksshow) | **GET** /api/v1/validation_checks/{id} | Get a single validation check|
|[**validationChecksStore**](#validationchecksstore) | **POST** /api/v1/validation_checks | Create a new validation check|
|[**validationChecksUpdate**](#validationchecksupdate) | **PUT** /api/v1/validation_checks/{id} | Update a validation check|

# **validationChecksDestroy**
> ValidationChecksDestroy200Response validationChecksDestroy()

Remove a validation check.

### Example

```typescript
import {
    ValidationChecksApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationChecksApi(configuration);

let id: number; //ID of the validation check (default to undefined)

const { status, data } = await apiInstance.validationChecksDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the validation check | defaults to undefined|


### Return type

**ValidationChecksDestroy200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation check deleted successfully |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Validation check not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationChecksIndex**
> Array<ValidationCheck> validationChecksIndex()

Retrieve all validation checks.

### Example

```typescript
import {
    ValidationChecksApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationChecksApi(configuration);

const { status, data } = await apiInstance.validationChecksIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<ValidationCheck>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation checks retrieved successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationChecksShow**
> ValidationCheck validationChecksShow()

Retrieve a specific validation check by ID.

### Example

```typescript
import {
    ValidationChecksApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationChecksApi(configuration);

let id: number; //ID of the validation check (default to undefined)

const { status, data } = await apiInstance.validationChecksShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the validation check | defaults to undefined|


### Return type

**ValidationCheck**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation check retrieved successfully |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Validation check not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationChecksStore**
> ValidationCheck validationChecksStore(validationChecksStoreRequest)

Create a new validation check entry.

### Example

```typescript
import {
    ValidationChecksApi,
    Configuration,
    ValidationChecksStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationChecksApi(configuration);

let validationChecksStoreRequest: ValidationChecksStoreRequest; //

const { status, data } = await apiInstance.validationChecksStore(
    validationChecksStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **validationChecksStoreRequest** | **ValidationChecksStoreRequest**|  | |


### Return type

**ValidationCheck**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Validation check created successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validationChecksUpdate**
> ValidationCheck validationChecksUpdate(validationChecksStoreRequest)

Edit an existing validation check.

### Example

```typescript
import {
    ValidationChecksApi,
    Configuration,
    ValidationChecksStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ValidationChecksApi(configuration);

let id: number; //ID of the validation check (default to undefined)
let validationChecksStoreRequest: ValidationChecksStoreRequest; //

const { status, data } = await apiInstance.validationChecksUpdate(
    id,
    validationChecksStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **validationChecksStoreRequest** | **ValidationChecksStoreRequest**|  | |
| **id** | [**number**] | ID of the validation check | defaults to undefined|


### Return type

**ValidationCheck**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Validation check updated successfully |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Validation check not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

