# UksaLiveFeed

Model representing UKSA live feed data

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the UKSA live feed record | [optional] [default to undefined]
**first_name** | **string** | First name of the individual | [optional] [default to undefined]
**last_name** | **string** | Last name of the individual | [optional] [default to undefined]
**organisation_name** | **string** | Name of the organisation | [optional] [default to undefined]
**accreditation_number** | **string** | Accreditation number | [optional] [default to undefined]
**accreditation_type** | **string** | Type of accreditation | [optional] [default to undefined]
**expiry_date** | **string** | Expiry date of the accreditation | [optional] [default to undefined]
**public_record** | **string** | Indicates whether the record is public | [optional] [default to undefined]
**stage** | **string** | Current stage of the accreditation process | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the record was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the record was last updated | [optional] [default to undefined]

## Example

```typescript
import { UksaLiveFeed } from '@hdruk/safepeopleregistry-api-sdk';

const instance: UksaLiveFeed = {
    id,
    first_name,
    last_name,
    organisation_name,
    accreditation_number,
    accreditation_type,
    expiry_date,
    public_record,
    stage,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
