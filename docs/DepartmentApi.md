# DepartmentApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**departmentDestroy**](#departmentdestroy) | **DELETE** /api/v1/departments/{id} | Delete a department|
|[**departmentIndex**](#departmentindex) | **GET** /api/v1/departments | Get a list of departments|
|[**departmentShow**](#departmentshow) | **GET** /api/v1/departments/{id} | Get a specific department by ID|
|[**departmentStore**](#departmentstore) | **POST** /api/v1/departments | Create a new department|
|[**departmentUpdate**](#departmentupdate) | **PUT** /api/v1/departments/{id} | Update an existing department|

# **departmentDestroy**
> AffiliationDestroy200Response departmentDestroy()


### Example

```typescript
import {
    DepartmentApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new DepartmentApi(configuration);

let id: number; //ID of the department (default to undefined)

const { status, data } = await apiInstance.departmentDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the department | defaults to undefined|


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
|**200** | Deleted |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Department not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **departmentIndex**
> Array<Department> departmentIndex()


### Example

```typescript
import {
    DepartmentApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new DepartmentApi(configuration);

const { status, data } = await apiInstance.departmentIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Department>**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **departmentShow**
> Department departmentShow()


### Example

```typescript
import {
    DepartmentApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new DepartmentApi(configuration);

let id: number; //ID of the department (default to undefined)

const { status, data } = await apiInstance.departmentShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the department | defaults to undefined|


### Return type

**Department**

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
|**404** | Department not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **departmentStore**
> AccreditationStoreByRegistryId201Response departmentStore(department)


### Example

```typescript
import {
    DepartmentApi,
    Configuration,
    Department
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new DepartmentApi(configuration);

let department: Department; //

const { status, data } = await apiInstance.departmentStore(
    department
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **department** | **Department**|  | |


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
|**201** | Created |  -  |
|**400** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **departmentUpdate**
> Department departmentUpdate(department)


### Example

```typescript
import {
    DepartmentApi,
    Configuration,
    Department
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new DepartmentApi(configuration);

let id: number; //ID of the department (default to undefined)
let department: Department; //

const { status, data } = await apiInstance.departmentUpdate(
    id,
    department
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **department** | **Department**|  | |
| **id** | [**number**] | ID of the department | defaults to undefined|


### Return type

**Department**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Updated |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Department not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

