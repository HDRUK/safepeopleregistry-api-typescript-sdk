# Custodian

Custodian model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**unique_identifier** | **string** | A unique identifier for Custodian\&#39;s within SOURSD | [optional] [default to undefined]
**contact_email** | **string** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**invite_accepted_at** | **string** |  | [optional] [default to undefined]
**invite_sent_at** | **string** |  | [optional] [default to undefined]
**idvt_required** | **boolean** |  | [optional] [default to undefined]
**gateway_app_id** | **string** |  | [optional] [default to undefined]
**gateway_client_id** | **string** |  | [optional] [default to undefined]
**client_id** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Custodian } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Custodian = {
    id,
    created_at,
    updated_at,
    name,
    unique_identifier,
    contact_email,
    enabled,
    invite_accepted_at,
    invite_sent_at,
    idvt_required,
    gateway_app_id,
    gateway_client_id,
    client_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
