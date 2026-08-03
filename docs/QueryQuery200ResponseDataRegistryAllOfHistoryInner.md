# QueryQuery200ResponseDataRegistryAllOfHistoryInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the history record | [optional] [default to undefined]
**affiliation_id** | **number** | ID of the affiliation associated with the history record | [optional] [default to undefined]
**endorsement_id** | **number** | ID of the endorsement associated with the history record | [optional] [default to undefined]
**infringement_id** | **number** | ID of the infringement associated with the history record | [optional] [default to undefined]
**project_id** | **number** | ID of the project associated with the history record | [optional] [default to undefined]
**access_key_id** | **number** | ID of the access key associated with the history record | [optional] [default to undefined]
**custodian_identifier** | **string** | Identifier for the custodian associated with the history record | [optional] [default to undefined]
**ledger_hash** | **string** | Hash of the ledger associated with the history record | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the history record was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the history record was last updated | [optional] [default to undefined]
**affiliation** | [**Affiliation**](Affiliation.md) |  | [optional] [default to undefined]
**project** | [**Project**](Project.md) |  | [optional] [default to undefined]

## Example

```typescript
import { QueryQuery200ResponseDataRegistryAllOfHistoryInner } from '@hdruk/safepeopleregistry-api-sdk';

const instance: QueryQuery200ResponseDataRegistryAllOfHistoryInner = {
    id,
    affiliation_id,
    endorsement_id,
    infringement_id,
    project_id,
    access_key_id,
    custodian_identifier,
    ledger_hash,
    created_at,
    updated_at,
    affiliation,
    project,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
