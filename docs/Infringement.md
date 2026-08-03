# Infringement

Model representing infringements

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the infringement | [optional] [default to undefined]
**reported_by** | **number** | ID of the user who reported the infringement | [optional] [default to undefined]
**comment** | **string** | Optional comment provided by the reporter | [optional] [default to undefined]
**raised_against** | **number** | ID of the entity the infringement is raised against | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the infringement was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the infringement was last updated | [optional] [default to undefined]

## Example

```typescript
import { Infringement } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Infringement = {
    id,
    reported_by,
    comment,
    raised_against,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
