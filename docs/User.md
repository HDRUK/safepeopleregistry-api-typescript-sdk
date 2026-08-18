# User

User model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**first_name** | **string** |  | [optional] [default to undefined]
**last_name** | **string** |  | [optional] [default to undefined]
**email** | **string** |  | [optional] [default to undefined]
**email_verified_at** | **string** |  | [optional] [default to undefined]
**consent_scrape** | **boolean** |  | [optional] [default to undefined]
**public_opt_in** | **boolean** |  | [optional] [default to undefined]
**organisation_id** | **number** |  | [optional] [default to undefined]
**orcid_scanning** | **number** |  | [optional] [default to undefined]
**orcid_scanning_completed_at** | **string** |  | [optional] [default to undefined]
**location** | **string** |  | [optional] [default to undefined]
**t_and_c_agreed** | **boolean** |  | [optional] [default to undefined]
**t_and_c_agreement_date** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { User } from '@hdruk/safepeopleregistry-api-sdk';

const instance: User = {
    id,
    created_at,
    updated_at,
    first_name,
    last_name,
    email,
    email_verified_at,
    consent_scrape,
    public_opt_in,
    organisation_id,
    orcid_scanning,
    orcid_scanning_completed_at,
    location,
    t_and_c_agreed,
    t_and_c_agreement_date,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
