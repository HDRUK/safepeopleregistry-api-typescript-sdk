# ValidationLog

Validation Log model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**entity_type** | **string** | Type of the primary entity associated with the validation log | [optional] [default to undefined]
**entity_id** | **number** | ID of the primary entity associated with the validation log | [optional] [default to undefined]
**secondary_entity_type** | **string** | Type of the secondary entity associated with the validation log | [optional] [default to undefined]
**secondary_entity_id** | **number** | ID of the secondary entity associated with the validation log | [optional] [default to undefined]
**tertiary_entity_type** | **string** | Type of the tertiary entity associated with the validation log | [optional] [default to undefined]
**tertiary_entity_id** | **number** | ID of the tertiary entity associated with the validation log | [optional] [default to undefined]
**name** | **string** | Name of the validation log entry | [optional] [default to undefined]
**completed_at** | **string** | Timestamp when the validation was completed (nullable) | [optional] [default to undefined]
**manually_confirmed** | **boolean** | Whether the validation was manually confirmed | [optional] [default to undefined]

## Example

```typescript
import { ValidationLog } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ValidationLog = {
    id,
    entity_type,
    entity_id,
    secondary_entity_type,
    secondary_entity_id,
    tertiary_entity_type,
    tertiary_entity_id,
    name,
    completed_at,
    manually_confirmed,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
