# ProjectHasCustodian

Pivot model representing the relationship between projects and custodians

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the project-custodian relationship | [optional] [default to undefined]
**project_id** | **number** | ID of the project | [optional] [default to undefined]
**custodian_id** | **number** | ID of the custodian | [optional] [default to undefined]
**approved** | **number** | Indicates whether the custodian is approved for the project (1 for approved, 0 for not approved) | [optional] [default to undefined]

## Example

```typescript
import { ProjectHasCustodian } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ProjectHasCustodian = {
    id,
    project_id,
    custodian_id,
    approved,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
