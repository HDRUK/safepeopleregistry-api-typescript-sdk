# PendingInvite

Model representing pending invites

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the pending invite | [optional] [default to undefined]
**user_id** | **number** | ID of the user associated with the invite | [optional] [default to undefined]
**organisation_id** | **number** | ID of the organisation associated with the invite | [optional] [default to undefined]
**status** | **string** | Status of the invite | [optional] [default to undefined]
**invite_accepted_at** | **string** | Timestamp when the invite was accepted | [optional] [default to undefined]
**invite_sent_at** | **string** | Timestamp when the invite was sent | [optional] [default to undefined]
**invite_code** | **string** | Unique code for the invite | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the invite record was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the invite record was last updated | [optional] [default to undefined]

## Example

```typescript
import { PendingInvite } from '@hdruk/safepeopleregistry-api-sdk';

const instance: PendingInvite = {
    id,
    user_id,
    organisation_id,
    status,
    invite_accepted_at,
    invite_sent_at,
    invite_code,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
