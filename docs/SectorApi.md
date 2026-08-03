# SectorApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**sectorDestroy**](#sectordestroy) | **DELETE** /api/v1/sectors/{id} | Delete a sector|
|[**sectorIndex**](#sectorindex) | **GET** /api/v1/sectors | Get a list of sectors|
|[**sectorShow**](#sectorshow) | **GET** /api/v1/sectors/{id} | Get a specific sector by ID|
|[**sectorStore**](#sectorstore) | **POST** /api/v1/sectors | Create a new sector|
|[**sectorUpdate**](#sectorupdate) | **PUT** /api/v1/sectors/{id} | Update an existing sector|

# **sectorDestroy**
> AffiliationDestroy200Response sectorDestroy()


### Example

```typescript
import {
    SectorApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SectorApi(configuration);

let id: number; //ID of the sector (default to undefined)

const { status, data } = await apiInstance.sectorDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the sector | defaults to undefined|


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
|**404** | Sector not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sectorIndex**
> Array<Sector> sectorIndex()


### Example

```typescript
import {
    SectorApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SectorApi(configuration);

const { status, data } = await apiInstance.sectorIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<Sector>**

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

# **sectorShow**
> Sector sectorShow()


### Example

```typescript
import {
    SectorApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SectorApi(configuration);

let id: number; //ID of the sector (default to undefined)

const { status, data } = await apiInstance.sectorShow(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the sector | defaults to undefined|


### Return type

**Sector**

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
|**404** | Sector not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sectorStore**
> AccreditationStoreByRegistryId201Response sectorStore(sector)


### Example

```typescript
import {
    SectorApi,
    Configuration,
    Sector
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SectorApi(configuration);

let sector: Sector; //

const { status, data } = await apiInstance.sectorStore(
    sector
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sector** | **Sector**|  | |


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

# **sectorUpdate**
> Sector sectorUpdate(sector)


### Example

```typescript
import {
    SectorApi,
    Configuration,
    Sector
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SectorApi(configuration);

let id: number; //ID of the sector (default to undefined)
let sector: Sector; //

const { status, data } = await apiInstance.sectorUpdate(
    id,
    sector
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sector** | **Sector**|  | |
| **id** | [**number**] | ID of the sector | defaults to undefined|


### Return type

**Sector**

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
|**404** | Sector not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

