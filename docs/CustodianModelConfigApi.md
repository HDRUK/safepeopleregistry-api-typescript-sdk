# CustodianModelConfigApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianModelConfigDestroy**](#custodianmodelconfigdestroy) | **DELETE** /api/v1/custodian_config/{id} | CustodianModelConfig@destroy|
|[**custodianModelConfigGetByCustodianID**](#custodianmodelconfiggetbycustodianid) | **GET** /api/v1/custodian_config/{id} | CustodianModelConfig@getByCustodianID|
|[**custodianModelConfigGetEntityModels**](#custodianmodelconfiggetentitymodels) | **GET** /api/v1/custodian_config/{custodianId}/entity_models | Get entity models for custodian config|
|[**custodianModelConfigStore**](#custodianmodelconfigstore) | **POST** /api/v1/custodian_config | CustodianModelConfig@store|
|[**custodianModelConfigUpdate**](#custodianmodelconfigupdate) | **PUT** /api/v1/custodian_config/{id} | CustodianModelConfig@update|
|[**custodianModelConfigUpdateEntityModels**](#custodianmodelconfigupdateentitymodels) | **PUT** /api/v1/custodian_config/{custodianId}/entity_models | Update a custodian\&#39;s entity models|

# **custodianModelConfigDestroy**
> AffiliationDestroy200Response custodianModelConfigDestroy()

Delete a CustodianModelConfig entry from the system

### Example

```typescript
import {
    CustodianModelConfigApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianModelConfigApi(configuration);

let id: number; //CustodianModelConfig entry ID (default to undefined)

const { status, data } = await apiInstance.custodianModelConfigDestroy(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | CustodianModelConfig entry ID | defaults to undefined|


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

# **custodianModelConfigGetByCustodianID**
> CustodianModelConfigGetByCustodianID200Response custodianModelConfigGetByCustodianID()

Return a list of Custodian config

### Example

```typescript
import {
    CustodianModelConfigApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianModelConfigApi(configuration);

let id: number; //CustodianModelConfig entry ID (default to undefined)

const { status, data } = await apiInstance.custodianModelConfigGetByCustodianID(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | CustodianModelConfig entry ID | defaults to undefined|


### Return type

**CustodianModelConfigGetByCustodianID200Response**

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

# **custodianModelConfigGetEntityModels**
> CustodianModelConfigGetEntityModels200Response custodianModelConfigGetEntityModels()

Retrieve entity models associated with custodian config based on the specified entity_model_type

### Example

```typescript
import {
    CustodianModelConfigApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianModelConfigApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let entityModelType: 'decision_model' | 'user_validation_rules' | 'org_validation_rules'; //Type of entity model to retrieve (default to undefined)

const { status, data } = await apiInstance.custodianModelConfigGetEntityModels(
    custodianId,
    entityModelType
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|
| **entityModelType** | [**&#39;decision_model&#39; | &#39;user_validation_rules&#39; | &#39;org_validation_rules&#39;**]**Array<&#39;decision_model&#39; &#124; &#39;user_validation_rules&#39; &#124; &#39;org_validation_rules&#39;>** | Type of entity model to retrieve | defaults to undefined|


### Return type

**CustodianModelConfigGetEntityModels200Response**

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

# **custodianModelConfigStore**
> CustodianModelConfigUpdate200Response custodianModelConfigStore(custodianModelConfig)

Create a CustodianModelConfig entry

### Example

```typescript
import {
    CustodianModelConfigApi,
    Configuration,
    CustodianModelConfig
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianModelConfigApi(configuration);

let custodianModelConfig: CustodianModelConfig; //CustodianModelConfig definition

const { status, data } = await apiInstance.custodianModelConfigStore(
    custodianModelConfig
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianModelConfig** | **CustodianModelConfig**| CustodianModelConfig definition | |


### Return type

**CustodianModelConfigUpdate200Response**

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
|**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodianModelConfigUpdate**
> CustodianModelConfigUpdate200Response custodianModelConfigUpdate(custodianModelConfig)

Update an CustodianModelConfig entry

### Example

```typescript
import {
    CustodianModelConfigApi,
    Configuration,
    CustodianModelConfig
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianModelConfigApi(configuration);

let id: number; //CustodianModelConfig entry ID (default to undefined)
let custodianModelConfig: CustodianModelConfig; //CustodianModelConfig definition

const { status, data } = await apiInstance.custodianModelConfigUpdate(
    id,
    custodianModelConfig
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianModelConfig** | **CustodianModelConfig**| CustodianModelConfig definition | |
| **id** | [**number**] | CustodianModelConfig entry ID | defaults to undefined|


### Return type

**CustodianModelConfigUpdate200Response**

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

# **custodianModelConfigUpdateEntityModels**
> CustodianModelConfigUpdateEntityModels200Response custodianModelConfigUpdateEntityModels(custodianModelConfigUpdateEntityModelsRequest)

Update the active status of specified custodian model configs for a given custodian

### Example

```typescript
import {
    CustodianModelConfigApi,
    Configuration,
    CustodianModelConfigUpdateEntityModelsRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianModelConfigApi(configuration);

let custodianId: number; //ID of the custodian (default to undefined)
let custodianModelConfigUpdateEntityModelsRequest: CustodianModelConfigUpdateEntityModelsRequest; //

const { status, data } = await apiInstance.custodianModelConfigUpdateEntityModels(
    custodianId,
    custodianModelConfigUpdateEntityModelsRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianModelConfigUpdateEntityModelsRequest** | **CustodianModelConfigUpdateEntityModelsRequest**|  | |
| **custodianId** | [**number**] | ID of the custodian | defaults to undefined|


### Return type

**CustodianModelConfigUpdateEntityModels200Response**

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
|**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

