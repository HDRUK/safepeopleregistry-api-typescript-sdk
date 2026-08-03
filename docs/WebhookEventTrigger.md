# WebhookEventTrigger

Model representing webhook event triggers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the webhook event trigger | [optional] [default to undefined]
**name** | **string** | Name of the webhook event trigger | [optional] [default to undefined]
**description** | **string** | Description of the webhook event trigger | [optional] [default to undefined]
**enabled** | **boolean** | Indicates whether the webhook event trigger is enabled | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the webhook event trigger was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the webhook event trigger was last updated | [optional] [default to undefined]

## Example

```typescript
import { WebhookEventTrigger } from '@hdruk/safepeopleregistry-api-sdk';

const instance: WebhookEventTrigger = {
    id,
    name,
    description,
    enabled,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
