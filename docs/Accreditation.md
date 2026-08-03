# Accreditation

Accreditation model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the accreditation | [optional] [default to undefined]
**associated_organisation_name** | **string** | Name of the associated organisation | [optional] [default to undefined]
**id_string** | **string** | ID string for the accreditation | [optional] [default to undefined]
**issue_date** | **string** | Date when the accreditation was issued | [optional] [default to undefined]
**expiry_date** | **string** | Date when the accreditation expires | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the accreditation was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the accreditation was last updated | [optional] [default to undefined]

## Example

```typescript
import { Accreditation } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Accreditation = {
    id,
    associated_organisation_name,
    id_string,
    issue_date,
    expiry_date,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
