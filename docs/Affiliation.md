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
**to** | **string** | Date affiliation ends (or ended). Null when there is no known end date | [optional] [default to undefined]
**end_date_recorded_at** | **string** | When the end date was recorded | [optional] [default to undefined]
**end_date_recorded_by** | **number** | The user who recorded the end date | [optional] [default to undefined]
**end_date_source** | **string** | Who recorded the end date. The organisation\&#39;s date wins over the user\&#39;s | [optional] [default to undefined]
**left_at** | **string** | When the leaver flow ran for this affiliation | [optional] [default to undefined]
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
    end_date_recorded_at,
    end_date_recorded_by,
    end_date_source,
    left_at,
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
