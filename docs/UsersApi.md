# UsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**usersStore**](#usersstore) | **POST** /api/v1/users | Users@store|

# **usersStore**
> UsersStore201Response usersStore(usersStoreRequest)

Create a User entry

### Example

```typescript
import {
    UsersApi,
    Configuration,
    UsersStoreRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let usersStoreRequest: UsersStoreRequest; //User definition

const { status, data } = await apiInstance.usersStore(
    usersStoreRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **usersStoreRequest** | **UsersStoreRequest**| User definition | |


### Return type

**UsersStore201Response**

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

