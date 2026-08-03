# ONSSubmissionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**oNSSubmissionReceiveCSV**](#onssubmissionreceivecsv) | **POST** /api/v1/ons-submissions/csv | Upload a CSV file for ONS submission|

# **oNSSubmissionReceiveCSV**
> ONSSubmissionReceiveCSV200Response oNSSubmissionReceiveCSV()


### Example

```typescript
import {
    ONSSubmissionApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ONSSubmissionApi(configuration);

let file: File; //CSV file to upload (optional) (default to undefined)

const { status, data } = await apiInstance.oNSSubmissionReceiveCSV(
    file
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **file** | [**File**] | CSV file to upload | (optional) defaults to undefined|


### Return type

**ONSSubmissionReceiveCSV200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | File uploaded successfully |  -  |
|**400** | File upload failed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

