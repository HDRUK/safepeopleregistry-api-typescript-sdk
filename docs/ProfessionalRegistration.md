# ProfessionalRegistration

Model representing professional registrations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the professional registration | [optional] [default to undefined]
**member_id** | **string** | Member ID associated with the professional registration | [optional] [default to undefined]
**name** | **string** | Name of the professional registration | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the professional registration was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the professional registration was last updated | [optional] [default to undefined]

## Example

```typescript
import { ProfessionalRegistration } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ProfessionalRegistration = {
    id,
    member_id,
    name,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
