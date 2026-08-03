# CustodianWebhookReceiver

Model representing webhook receivers for custodians

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the webhook receiver | [optional] [default to undefined]
**custodian_id** | **number** | ID of the custodian associated with the webhook receiver | [optional] [default to undefined]
**url** | **string** | URL of the webhook receiver | [optional] [default to undefined]
**webhook_event** | **number** | ID of the webhook event associated with the receiver | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the webhook receiver was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the webhook receiver was last updated | [optional] [default to undefined]

## Example

```typescript
import { CustodianWebhookReceiver } from '@hdruk/safepeopleregistry-api-sdk';

const instance: CustodianWebhookReceiver = {
    id,
    custodian_id,
    url,
    webhook_event,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
