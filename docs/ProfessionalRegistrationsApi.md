# ProfessionalRegistrationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**professionalRegistrationsUpdate**](#professionalregistrationsupdate) | **PUT** /api/v1/professional_registrations/{id} | Professional Registrations@update|

# **professionalRegistrationsUpdate**
> ProfessionalRegistrationsUpdate200Response professionalRegistrationsUpdate(professionalRegistrationsUpdateRequest)

Update a Professional Registrations entry

### Example

```typescript
import {
    ProfessionalRegistrationsApi,
    Configuration,
    ProfessionalRegistrationsUpdateRequest
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ProfessionalRegistrationsApi(configuration);

let id: number; //Professional Registrations entry ID (default to undefined)
let professionalRegistrationsUpdateRequest: ProfessionalRegistrationsUpdateRequest; //Professional Registrations definition

const { status, data } = await apiInstance.professionalRegistrationsUpdate(
    id,
    professionalRegistrationsUpdateRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **professionalRegistrationsUpdateRequest** | **ProfessionalRegistrationsUpdateRequest**| Professional Registrations definition | |
| **id** | [**number**] | Professional Registrations entry ID | defaults to undefined|


### Return type

**ProfessionalRegistrationsUpdate200Response**

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

