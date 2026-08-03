# NotificationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**notificationsGetNotificationCounts**](#notificationsgetnotificationcounts) | **GET** /api/v1/users/{id}/notifications/count | Get notification counts for a specific user|
|[**notificationsGetUserNotifications**](#notificationsgetusernotifications) | **GET** /api/v1/users/{id}/notifications | Get notifications for a specific user|
|[**notificationsMarkUserNotificationAsRead**](#notificationsmarkusernotificationasread) | **PATCH** /api/v1/users/{id}/notifications/{notificationId}/read | Mark a specific notification as read|
|[**notificationsMarkUserNotificationAsUnread**](#notificationsmarkusernotificationasunread) | **PATCH** /api/v1/users/{id}/notifications/{notificationId}/unread | Mark a specific notification as unread|
|[**notificationsMarkUserNotificationsAsRead**](#notificationsmarkusernotificationsasread) | **PATCH** /api/v1/users/{id}/notifications/read | Mark all notifications as read for a specific user|

# **notificationsGetNotificationCounts**
> NotificationsGetNotificationCounts200Response notificationsGetNotificationCounts()

Retrieve the total, read, and unread notification counts for a given user.

### Example

```typescript
import {
    NotificationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationsApi(configuration);

let id: number; //User ID (default to undefined)

const { status, data } = await apiInstance.notificationsGetNotificationCounts(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User ID | defaults to undefined|


### Return type

**NotificationsGetNotificationCounts200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**401** | Unauthorized |  -  |
|**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notificationsGetUserNotifications**
> NotificationsGetUserNotifications200Response notificationsGetUserNotifications()

Retrieves notifications for a user, with an optional filter for read/unread notifications.

### Example

```typescript
import {
    NotificationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationsApi(configuration);

let id: number; //User ID (default to undefined)
let status: 'read' | 'unread'; //Filter notifications by status (read/unread) (optional) (default to undefined)

const { status, data } = await apiInstance.notificationsGetUserNotifications(
    id,
    status
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User ID | defaults to undefined|
| **status** | [**&#39;read&#39; | &#39;unread&#39;**]**Array<&#39;read&#39; &#124; &#39;unread&#39;>** | Filter notifications by status (read/unread) | (optional) defaults to undefined|


### Return type

**NotificationsGetUserNotifications200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notificationsMarkUserNotificationAsRead**
> NotificationsMarkUserNotificationAsRead200Response notificationsMarkUserNotificationAsRead()


### Example

```typescript
import {
    NotificationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationsApi(configuration);

let id: number; //User ID (default to undefined)
let notificationId: string; //Notification ID (default to undefined)

const { status, data } = await apiInstance.notificationsMarkUserNotificationAsRead(
    id,
    notificationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User ID | defaults to undefined|
| **notificationId** | [**string**] | Notification ID | defaults to undefined|


### Return type

**NotificationsMarkUserNotificationAsRead200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Notification marked as read |  -  |
|**404** | User or notification not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notificationsMarkUserNotificationAsUnread**
> notificationsMarkUserNotificationAsUnread()


### Example

```typescript
import {
    NotificationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationsApi(configuration);

let id: number; //User ID (default to undefined)
let notificationId: string; //Notification ID (default to undefined)

const { status, data } = await apiInstance.notificationsMarkUserNotificationAsUnread(
    id,
    notificationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User ID | defaults to undefined|
| **notificationId** | [**string**] | Notification ID | defaults to undefined|


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
|**200** | Notification marked as unread |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notificationsMarkUserNotificationsAsRead**
> NotificationsMarkUserNotificationsAsRead200Response notificationsMarkUserNotificationsAsRead()


### Example

```typescript
import {
    NotificationsApi,
    Configuration
} from '@hdruk/safepeopleregistry-api-sdk';

const configuration = new Configuration();
const apiInstance = new NotificationsApi(configuration);

let id: number; //User ID (default to undefined)

const { status, data } = await apiInstance.notificationsMarkUserNotificationsAsRead(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**number**] | User ID | defaults to undefined|


### Return type

**NotificationsMarkUserNotificationsAsRead200Response**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Notifications marked as read |  -  |
|**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

