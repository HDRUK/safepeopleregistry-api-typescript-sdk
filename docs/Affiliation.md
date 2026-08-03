# Affiliation

Affiliation model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**organisation_id** | **number** | Organisational link | [optional] [default to undefined]
**member_id** | **string** | Member ID UUID | [optional] [default to undefined]
**relationship** | **string** | Textual representation of affiliation relationship | [optional] [default to undefined]
**from** | **string** | Date affiliation commenced | [optional] [default to undefined]
**to** | **string** | Date affiliation concluded | [optional] [default to undefined]
**department** | **string** | Department worked during affiliation | [optional] [default to undefined]
**role** | **string** | Role held during affiliation | [optional] [default to undefined]
**email** | **string** | Professional email held during affiliation | [optional] [default to undefined]
**ror** | **string** | The ROR.org identifier for this affiliation institute | [optional] [default to undefined]
**registry_id** | **number** | The Registry primary key associated with this affiliation | [optional] [default to undefined]
**current_employer** | **boolean** | Flag indicating if affiliation is for the current employer | [optional] [default to undefined]
**verification_code** | **string** | Unique verification code issued for confirmation | [optional] [default to undefined]
**verification_sent_at** | **string** | Timestamp when verification code was sent | [optional] [default to undefined]
**verification_confirmed_at** | **string** | Timestamp when verification was confirmed | [optional] [default to undefined]
**is_verified** | **boolean** | Flag indicating if affiliation is verified | [optional] [default to undefined]

## Example

```typescript
import { Affiliation } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Affiliation = {
    id,
    created_at,
    updated_at,
    organisation_id,
    member_id,
    relationship,
    from,
    to,
    department,
    role,
    email,
    ror,
    registry_id,
    current_employer,
    verification_code,
    verification_sent_at,
    verification_confirmed_at,
    is_verified,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
