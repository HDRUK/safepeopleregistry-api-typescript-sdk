# Identity

Model representing identity records

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the identity record | [optional] [default to undefined]
**registry_id** | **number** | ID of the registry associated with the identity record | [optional] [default to undefined]
**address_1** | **string** | First line of the address | [optional] [default to undefined]
**address_2** | **string** | Second line of the address | [optional] [default to undefined]
**town** | **string** | Town of the address | [optional] [default to undefined]
**county** | **string** | County of the address | [optional] [default to undefined]
**country** | **string** | Country of the address | [optional] [default to undefined]
**postcode** | **string** | Postcode of the address | [optional] [default to undefined]
**dob** | **string** | Date of birth | [optional] [default to undefined]
**idvt_success** | **number** | Indicates whether IDVT was successful (1 for success, 0 for failure) | [optional] [default to undefined]
**idvt_identification_number** | **string** | Identification number from IDVT | [optional] [default to undefined]
**idvt_document_type** | **string** | Type of document used for IDVT | [optional] [default to undefined]
**idvt_document_number** | **string** | Document number used for IDVT | [optional] [default to undefined]
**idvt_document_country** | **string** | Country of the document used for IDVT | [optional] [default to undefined]
**idvt_document_valid_until** | **string** | Validity date of the document used for IDVT | [optional] [default to undefined]
**idvt_document_first_name** | **string** | First name on the document used for IDVT | [optional] [default to undefined]
**idvt_document_valid_last_name** | **string** | Last name on the document used for IDVT | [optional] [default to undefined]
**idvt_attempt_id** | **string** | ID of the IDVT attempt | [optional] [default to undefined]
**idvt_context_id** | **string** | Context ID for IDVT | [optional] [default to undefined]
**idvt_document_dob** | **string** | Date of birth on the document used for IDVT | [optional] [default to undefined]
**idvt_context** | **string** | Context of the IDVT process | [optional] [default to undefined]
**idvt_completed_at** | **string** | Timestamp when IDVT was completed | [optional] [default to undefined]
**idvt_result_text** | **string** | Result text of the IDVT process | [optional] [default to undefined]
**idvt_started_at** | **string** | Timestamp when IDVT was started | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the identity record was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the identity record was last updated | [optional] [default to undefined]
**deleted_at** | **string** | Timestamp when the identity record was deleted | [optional] [default to undefined]

## Example

```typescript
import { Identity } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Identity = {
    id,
    registry_id,
    address_1,
    address_2,
    town,
    county,
    country,
    postcode,
    dob,
    idvt_success,
    idvt_identification_number,
    idvt_document_type,
    idvt_document_number,
    idvt_document_country,
    idvt_document_valid_until,
    idvt_document_first_name,
    idvt_document_valid_last_name,
    idvt_attempt_id,
    idvt_context_id,
    idvt_document_dob,
    idvt_context,
    idvt_completed_at,
    idvt_result_text,
    idvt_started_at,
    created_at,
    updated_at,
    deleted_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
