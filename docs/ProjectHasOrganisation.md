# ProjectHasOrganisation

Relation between a project and an organisation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**project_id** | **number** | ID of the related project | [default to undefined]
**organisation_id** | **number** | ID of the related organisation | [default to undefined]
**organisation** | [**Organisation**](Organisation.md) |  | [optional] [default to undefined]
**project** | [**Project**](Project.md) |  | [optional] [default to undefined]

## Example

```typescript
import { ProjectHasOrganisation } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ProjectHasOrganisation = {
    id,
    project_id,
    organisation_id,
    organisation,
    project,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
