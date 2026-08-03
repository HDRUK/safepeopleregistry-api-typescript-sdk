# Experience

Model representing experiences

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the experience | [optional] [default to undefined]
**project_id** | **number** | ID of the project associated with the experience | [optional] [default to undefined]
**from** | **string** | Start date of the experience | [optional] [default to undefined]
**to** | **string** | End date of the experience | [optional] [default to undefined]
**organisation_id** | **number** | ID of the organisation associated with the experience | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the experience was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the experience was last updated | [optional] [default to undefined]

## Example

```typescript
import { Experience } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Experience = {
    id,
    project_id,
    from,
    to,
    organisation_id,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
