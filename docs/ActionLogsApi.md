# ActionLogsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**actionLogsGetEntityActionLog**](#actionlogsgetentityactionlog) | **GET** /api/v1/{entity}/{id}/action_log | Get Action Logs for an Entity|
|[**actionLogsUpdate**](#actionlogsupdate) | **PUT** /api/v1/action_logs/{id} | Update an Action Log|

# **actionLogsGetEntityActionLog**
> ActionLogsGetEntityActionLog200Response actionLogsGetEntityActionLog()

Retrieve action logs for a given entity type (users, organisations) by ID.

### Example

```typescript
import {
    ActionLogsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ActionLogsApi(configuration);

let entity: string; //The entity type (e.g., users, organisations) (default to undefined)
let id: number; //The ID of the entity (default to undefined)

const { status, data } = await apiInstance.actionLogsGetEntityActionLog(
    entity,
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **entity** | [**string**] | The entity type (e.g., users, organisations) | defaults to undefined|
| **id** | [**number**] | The ID of the entity | defaults to undefined|


### Return type

**ActionLogsGetEntityActionLog200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response with action logs |  -  |
|**404** | No action logs found for this entity |  -  |
|**400** | Invalid entity type |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **actionLogsUpdate**
> ActionLogsUpdate200Response actionLogsUpdate()

Update an action log entry, including marking it as complete or incomplete.

### Example

```typescript
import {
    ActionLogsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new ActionLogsApi(configuration);

let id: number; //ID of the action log (default to undefined)
let complete: boolean; //Mark as complete (optional) (default to undefined)
let incomplete: boolean; //Mark as incomplete (optional) (default to undefined)

const { status, data } = await apiInstance.actionLogsUpdate(
    id,
    complete,
    incomplete
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | ID of the action log | defaults to undefined|
| **complete** | [**boolean**] | Mark as complete | (optional) defaults to undefined|
| **incomplete** | [**boolean**] | Mark as incomplete | (optional) defaults to undefined|


### Return type

**ActionLogsUpdate200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Action status updated successfully |  -  |
|**404** | Action log not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

