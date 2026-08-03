# ModelState

Model representing the state of a model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the model state | [optional] [default to undefined]
**state_id** | **number** | ID of the state associated with the model state | [optional] [default to undefined]
**stateable_type** | **string** | Type of the model associated with the state | [optional] [default to undefined]
**stateable_id** | **number** | ID of the model associated with the state | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the model state was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the model state was last updated | [optional] [default to undefined]

## Example

```typescript
import { ModelState } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ModelState = {
    id,
    state_id,
    stateable_type,
    stateable_id,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
