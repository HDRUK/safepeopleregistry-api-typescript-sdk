# UserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**userDestroy**](#userdestroy) | **DELETE** /api/v1/users/{id} | User@destroy|
|[**userIndex**](#userindex) | **GET** /api/v1/users | User@index|
|[**userShow**](#usershow) | **GET** /api/v1/users/{id} | User@show|
|[**userUpdate**](#userupdate) | **PUT** /api/v1/users/{id} | User@update|

# **userDestroy**
> AffiliationDestroy200Response userDestroy()

Delete a User entry from the system

### Example

```typescript
import {
    UserApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: number; //User entry ID (default to undefined)

const { status, data } = await apiInstance.userDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User entry ID | defaults to undefined|


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
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **userIndex**
> UserIndex200Response userIndex()

Return a list of Users

### Example

```typescript
import {
    UserApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

const { status, data } = await apiInstance.userIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserIndex200Response**

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

# **userShow**
> UserShow200Response userShow()

Return a User entry by ID

### Example

```typescript
import {
    UserApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: number; //User ID (default to undefined)

const { status, data } = await apiInstance.userShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User ID | defaults to undefined|


### Return type

**UserShow200Response**

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

# **userUpdate**
> UserUpdate200Response userUpdate(userUpdateRequest)

Edit a User entry

### Example

```typescript
import {
    UserApi,
    Configuration,
    UserUpdateRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: number; //User ID (default to undefined)
let userUpdateRequest: UserUpdateRequest; //User definition

const { status, data } = await apiInstance.userUpdate(
    id,
    userUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userUpdateRequest** | **UserUpdateRequest**| User definition | |
| **id** | [**number**] | User ID | defaults to undefined|


### Return type

**UserUpdate200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**404** | Not found response |  -  |
|**200** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

