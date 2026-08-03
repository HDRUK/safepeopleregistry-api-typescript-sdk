# CustodianUsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**custodianUsersIndex**](#custodianusersindex) | **GET** /api/v1/custodian_users | Return a list of Custodian Users|

# **custodianUsersIndex**
> CustodianUsersIndex200Response custodianUsersIndex()

Return a list of Custodian Users

### Example

```typescript
import {
    CustodianUsersApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new CustodianUsersApi(configuration);

const { status, data } = await apiInstance.custodianUsersIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CustodianUsersIndex200Response**

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

