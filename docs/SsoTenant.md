# SsoTenant

An enterprise customer\'s SAML Identity Provider connection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**idp_alias** | **string** |  | [optional] [default to undefined]
**metadata_url** | **string** |  | [optional] [default to undefined]
**entity_id** | **string** |  | [optional] [default to undefined]
**metadata_imported_at** | **string** |  | [optional] [default to undefined]
**enabled** | **boolean** |  | [optional] [default to undefined]
**sp_entity_id** | **string** | Keycloak\&#39;s own SP entity ID - null until approved. Register this as the SAML Identifier on the customer\&#39;s IdP. | [optional] [default to undefined]
**sp_acs_url** | **string** | Keycloak\&#39;s ACS/reply URL for this tenant - null until approved. | [optional] [default to undefined]
**sp_metadata_url** | **string** | Downloadable SP metadata descriptor most IdPs can import directly - null until approved. | [optional] [default to undefined]
**status** | **string** | One of pending, approved, rejected | [optional] [default to undefined]
**submitted_by_user_id** | **number** | ID of the user who submitted this tenant for approval | [optional] [default to undefined]
**rejected_reason** | **string** | Reason given when status is rejected - null otherwise | [optional] [default to undefined]

## Example

```typescript
import { SsoTenant } from '@hdruk/safepeopleregistry-api-sdk';

const instance: SsoTenant = {
    id,
    created_at,
    updated_at,
    name,
    idp_alias,
    metadata_url,
    entity_id,
    metadata_imported_at,
    enabled,
    sp_entity_id,
    sp_acs_url,
    sp_metadata_url,
    status,
    submitted_by_user_id,
    rejected_reason,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
