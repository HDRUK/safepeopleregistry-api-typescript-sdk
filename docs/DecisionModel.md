# DecisionModel

Model representing decision models

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the decision model | [optional] [default to undefined]
**model_type** | **string** | Type of the model associated with the decision | [default to undefined]
**conditions** | **string** | Conditions for the decision model | [default to undefined]
**rule_class** | **string** | Class defining the rules for the decision model | [default to undefined]
**description** | **string** | Description of the decision model | [optional] [default to undefined]
**decision_model_type_id** | **number** | ID of the decision model type associated with the decision | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the decision model was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the decision model was last updated | [optional] [default to undefined]

## Example

```typescript
import { DecisionModel } from '@hdruk/safepeopleregistry-api-sdk';

const instance: DecisionModel = {
    id,
    model_type,
    conditions,
    rule_class,
    description,
    decision_model_type_id,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
