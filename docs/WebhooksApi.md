# WebhooksApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**webhooksCreateReceiver**](#webhookscreatereceiver) | **POST** /api/v1/webhooks/receivers | Create a new webhook receiver|
|[**webhooksDeleteReceiver**](#webhooksdeletereceiver) | **DELETE** /api/v1/webhooks/receivers/{custodianId} | Delete a webhook receiver|
|[**webhooksGetAllEventTriggers**](#webhooksgetalleventtriggers) | **GET** /api/v1/webhooks/event-triggers | Get all webhook event triggers|
|[**webhooksGetAllReceivers**](#webhooksgetallreceivers) | **GET** /api/v1/webhooks/receivers | Get all webhook receivers|
|[**webhooksGetReceiversByCustodian**](#webhooksgetreceiversbycustodian) | **GET** /api/v1/webhooks/receivers/{custodianId} | Get webhook receivers by custodian|
|[**webhooksSendgrid**](#webhookssendgrid) | **GET** /api/v1/webhooks/sendgrid | Get sendgrid webhook event triggers|
|[**webhooksUpdateReceiver**](#webhooksupdatereceiver) | **PUT** /api/v1/webhooks/receivers/{custodianId} | Update a webhook receiver|

# **webhooksCreateReceiver**
> WebhooksCreateReceiver201Response webhooksCreateReceiver(webhooksCreateReceiverRequest)

Creates a new webhook receiver for a custodian

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    WebhooksCreateReceiverRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let webhooksCreateReceiverRequest: WebhooksCreateReceiverRequest; //

const { status, data } = await apiInstance.webhooksCreateReceiver(
    webhooksCreateReceiverRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **webhooksCreateReceiverRequest** | **WebhooksCreateReceiverRequest**|  | |


### Return type

**WebhooksCreateReceiver201Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful operation |  -  |
|**422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooksDeleteReceiver**
> EducationDestroyByRegistryId200Response webhooksDeleteReceiver(webhooksDeleteReceiverRequest)

Deletes a specific webhook receiver for a custodian

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    WebhooksDeleteReceiverRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let custodianId: number; // (default to undefined)
let webhooksDeleteReceiverRequest: WebhooksDeleteReceiverRequest; //

const { status, data } = await apiInstance.webhooksDeleteReceiver(
    custodianId,
    webhooksDeleteReceiverRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **webhooksDeleteReceiverRequest** | **WebhooksDeleteReceiverRequest**|  | |
| **custodianId** | [**number**] |  | defaults to undefined|


### Return type

**EducationDestroyByRegistryId200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Webhook receiver not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooksGetAllEventTriggers**
> WebhooksGetAllEventTriggers200Response webhooksGetAllEventTriggers()

Returns all webhook event triggers

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

const { status, data } = await apiInstance.webhooksGetAllEventTriggers();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**WebhooksGetAllEventTriggers200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooksGetAllReceivers**
> WebhooksGetAllReceivers200Response webhooksGetAllReceivers()

Returns all webhook receivers with their associated event trigger details

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

const { status, data } = await apiInstance.webhooksGetAllReceivers();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**WebhooksGetAllReceivers200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooksGetReceiversByCustodian**
> WebhooksGetAllReceivers200Response webhooksGetReceiversByCustodian()

Returns all webhook receivers for a specific custodian with their associated event trigger details

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let custodianId: number; // (default to undefined)

const { status, data } = await apiInstance.webhooksGetReceiversByCustodian(
    custodianId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **custodianId** | [**number**] |  | defaults to undefined|


### Return type

**WebhooksGetAllReceivers200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |
|**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooksSendgrid**
> webhooksSendgrid()

Returns sendgrid webhook event triggers

### Example

```typescript
import {
    WebhooksApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

const { status, data } = await apiInstance.webhooksSendgrid();
```

### Parameters
This endpoint does not have any parameters.


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooksUpdateReceiver**
> EducationDestroyByRegistryId200Response webhooksUpdateReceiver(webhooksUpdateReceiverRequest)

Updates a specific webhook receiver for a custodian

### Example

```typescript
import {
    WebhooksApi,
    Configuration,
    WebhooksUpdateReceiverRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new WebhooksApi(configuration);

let custodianId: number; // (default to undefined)
let webhooksUpdateReceiverRequest: WebhooksUpdateReceiverRequest; //

const { status, data } = await apiInstance.webhooksUpdateReceiver(
    custodianId,
    webhooksUpdateReceiverRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **webhooksUpdateReceiverRequest** | **WebhooksUpdateReceiverRequest**|  | |
| **custodianId** | [**number**] |  | defaults to undefined|


### Return type

**EducationDestroyByRegistryId200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful operation |  -  |
|**400** | Invalid argument(s) |  -  |
|**404** | Webhook receiver not found |  -  |
|**422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

