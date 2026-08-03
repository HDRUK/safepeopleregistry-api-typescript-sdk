# CustodianHasProjectOrganisation

Custodian approval status for a project organisation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [readonly] [default to undefined]
**project_has_organisation_id** | **number** | ID of the project organisation | [default to undefined]
**custodian_id** | **number** | ID of the custodian | [default to undefined]
**approved** | **boolean** | Approval flag | [optional] [default to undefined]
**comment** | **string** | Optional comment | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**projectOrganisation** | [**ProjectHasOrganisation**](ProjectHasOrganisation.md) |  | [optional] [default to undefined]
**custodian** | [**Custodian**](Custodian.md) |  | [optional] [default to undefined]

## Example

```typescript
import { CustodianHasProjectOrganisation } from '@hdruk/safepeopleregistry-api-sdk';

const instance: CustodianHasProjectOrganisation = {
    id,
    project_has_organisation_id,
    custodian_id,
    approved,
    comment,
    created_at,
    updated_at,
    projectOrganisation,
    custodian,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
