# SsoTenantDomain

An email domain routed to a Registry SSO tenant\'s Identity Provider

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**sso_tenant_id** | **number** |  | [optional] [default to undefined]
**domain** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { SsoTenantDomain } from '@hdruk/safepeopleregistry-api-sdk';

const instance: SsoTenantDomain = {
    id,
    sso_tenant_id,
    domain,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
