# OrganisationHasCustodianPermission

Pivot model representing the relationship between organisations, custodians, and permissions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organisation_id** | **number** | ID of the organisation | [optional] [default to undefined]
**permission_id** | **number** | ID of the permission | [optional] [default to undefined]
**custodian_id** | **number** | ID of the custodian | [optional] [default to undefined]

## Example

```typescript
import { OrganisationHasCustodianPermission } from '@hdruk/safepeopleregistry-api-sdk';

const instance: OrganisationHasCustodianPermission = {
    organisation_id,
    permission_id,
    custodian_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
