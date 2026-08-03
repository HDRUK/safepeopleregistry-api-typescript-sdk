# ValidationCheck

Model representing validation checks

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the validation check | [optional] [default to undefined]
**name** | **string** | Name of the validation check | [default to undefined]
**description** | **string** | Description of the validation check | [default to undefined]
**applies_to** | **string** | Context to which the validation check applies | [default to undefined]
**enabled** | **boolean** | Indicates whether the validation check is enabled | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the validation check was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the validation check was last updated | [optional] [default to undefined]
**custodian_id** | **number** | Custodian id or null | [optional] [default to undefined]

## Example

```typescript
import { ValidationCheck } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ValidationCheck = {
    id,
    name,
    description,
    applies_to,
    enabled,
    created_at,
    updated_at,
    custodian_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
