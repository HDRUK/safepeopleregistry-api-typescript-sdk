# ValidationLogComment

Comments on validation logs

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**validation_log_id** | **number** | ID of the associated validation log | [optional] [default to undefined]
**user_id** | **number** | ID of the user who made the comment | [optional] [default to undefined]
**comment** | **string** | The comment text | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the comment was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the comment was last updated | [optional] [default to undefined]

## Example

```typescript
import { ValidationLogComment } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ValidationLogComment = {
    id,
    validation_log_id,
    user_id,
    comment,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
