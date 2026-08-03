# PendingInvitesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**pendingInvitesIndex**](#pendinginvitesindex) | **GET** /api/v1/pending_invites | PendingInvite@index|

# **pendingInvitesIndex**
> PendingInvitesIndex200Response pendingInvitesIndex()

Return a list of pending invites

### Example

```typescript
import {
    PendingInvitesApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new PendingInvitesApi(configuration);

const { status, data } = await apiInstance.pendingInvitesIndex();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**PendingInvitesIndex200Response**

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

