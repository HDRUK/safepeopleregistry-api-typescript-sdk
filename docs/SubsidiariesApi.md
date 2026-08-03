# SubsidiariesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**subsidiariesDestroy**](#subsidiariesdestroy) | **DELETE** /api/v1/subsidiaries/{subsidiaryId}/organisations/{organisationId} | subsidiaries@destroy|
|[**subsidiariesStore**](#subsidiariesstore) | **POST** /api/v1/subsidiaries/organisations/{organisationId} | subsidiaries@store|
|[**subsidiariesUpdate**](#subsidiariesupdate) | **PUT** /api/v1/subsidiaries/{subsidiaryId}/organisations/{organisationId} | subsidiaries@update|

# **subsidiariesDestroy**
> AffiliationDestroy200Response subsidiariesDestroy()

Delete an subsidiary entry from the system

### Example

```typescript
import {
    SubsidiariesApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SubsidiariesApi(configuration);

let organisationId: number; //organisations entry ID (default to undefined)
let subsidiaryId: number; //subsidiary entry ID (default to undefined)

const { status, data } = await apiInstance.subsidiariesDestroy(
    organisationId,
    subsidiaryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **organisationId** | [**number**] | organisations entry ID | defaults to undefined|
| **subsidiaryId** | [**number**] | subsidiary entry ID | defaults to undefined|


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

# **subsidiariesStore**
> SubsidiariesStore201Response subsidiariesStore(subsidiary)

Create a subsidiary entry

### Example

```typescript
import {
    SubsidiariesApi,
    Configuration,
    Subsidiary
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SubsidiariesApi(configuration);

let organisationId: number; //organisations entry ID (default to undefined)
let subsidiary: Subsidiary; //subsidiary definition

const { status, data } = await apiInstance.subsidiariesStore(
    organisationId,
    subsidiary
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **subsidiary** | **Subsidiary**| subsidiary definition | |
| **organisationId** | [**number**] | organisations entry ID | defaults to undefined|


### Return type

**SubsidiariesStore201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Success |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Not found response |  -  |
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subsidiariesUpdate**
> SubsidiariesStore201Response subsidiariesUpdate(subsidiary)

Update a subsidiary entry

### Example

```typescript
import {
    SubsidiariesApi,
    Configuration,
    Subsidiary
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new SubsidiariesApi(configuration);

let organisationId: number; //organisations entry ID (default to undefined)
let subsidiaryId: number; //subsidiary entry ID (default to undefined)
let subsidiary: Subsidiary; //subsidiary definition

const { status, data } = await apiInstance.subsidiariesUpdate(
    organisationId,
    subsidiaryId,
    subsidiary
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **subsidiary** | **Subsidiary**| subsidiary definition | |
| **organisationId** | [**number**] | organisations entry ID | defaults to undefined|
| **subsidiaryId** | [**number**] | subsidiary entry ID | defaults to undefined|


### Return type

**SubsidiariesStore201Response**

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

