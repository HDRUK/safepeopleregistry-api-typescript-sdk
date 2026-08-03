# ActionLog

Action Log model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**entity_type** | **string** | Type of the entity associated with the action log | [optional] [default to undefined]
**entity_id** | **number** | ID of the entity associated with the action log | [optional] [default to undefined]
**action** | **string** | Description of the action performed | [optional] [default to undefined]
**completed_at** | **string** | Timestamp when the action was completed (nullable) | [optional] [default to undefined]

## Example

```typescript
import { ActionLog } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ActionLog = {
    id,
    entity_type,
    entity_id,
    action,
    completed_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
