# EntityModel

Model representing entity models

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the entity model | [optional] [default to undefined]
**name** | **string** | Name of the entity model | [optional] [default to undefined]
**description** | **string** | Description of the entity model | [optional] [default to undefined]
**entity_model_type_id** | **number** | ID of the entity model type associated with this model | [optional] [default to undefined]
**calls_file** | **boolean** | Indicates whether the model calls a file | [optional] [default to undefined]
**file_path** | **string** | Path to the file called by the model | [optional] [default to undefined]
**calls_operation** | **boolean** | Indicates whether the model calls an operation | [optional] [default to undefined]
**operation** | **string** | Operation called by the model | [optional] [default to undefined]
**active** | **number** | Indicates whether the model is active (1 for active, 0 for inactive) | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the entity model was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the entity model was last updated | [optional] [default to undefined]

## Example

```typescript
import { EntityModel } from '@hdruk/safepeopleregistry-api-sdk';

const instance: EntityModel = {
    id,
    name,
    description,
    entity_model_type_id,
    calls_file,
    file_path,
    calls_operation,
    operation,
    active,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
