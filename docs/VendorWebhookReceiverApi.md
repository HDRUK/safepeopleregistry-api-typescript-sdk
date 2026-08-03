# VendorWebhookReceiverApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**vendorWebhookReceiverReceive**](#vendorwebhookreceiverreceive) | **POST** /api/v1/vendor-webhooks/{provider} | Receive a webhook callback from a vendor|

# **vendorWebhookReceiverReceive**
> VendorWebhookReceiverReceive200Response vendorWebhookReceiverReceive(body)


### Example

```typescript
import {
    VendorWebhookReceiverApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new VendorWebhookReceiverApi(configuration);

let provider: string; //Name of the vendor providing the webhook (default to undefined)
let body: object; //

const { status, data } = await apiInstance.vendorWebhookReceiverReceive(
    provider,
    body
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **body** | **object**|  | |
| **provider** | [**string**] | Name of the vendor providing the webhook | defaults to undefined|


### Return type

**VendorWebhookReceiverReceive200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Webhook processed successfully |  -  |
|**400** | Invalid argument(s) |  -  |
|**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

