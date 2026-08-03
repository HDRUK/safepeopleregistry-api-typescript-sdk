# ProjectDetail

ProjectDetail model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**project_id** | **number** | Primary key of associated Project for this ProjectDetail | [optional] [default to undefined]
**datasets** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**other_approval_committees** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**data_sensitivity_level** | **string** |  | [optional] [default to undefined]
**legal_basis_for_data_article6** | **string** |  | [optional] [default to undefined]
**duty_of_confidentiality** | **boolean** |  | [optional] [default to undefined]
**national_data_optout** | **boolean** |  | [optional] [default to undefined]
**request_frequency** | **string** |  | [optional] [default to undefined]
**dataset_linkage_description** | **string** |  | [optional] [default to undefined]
**data_minimisation** | **string** |  | [optional] [default to undefined]
**data_use_description** | **string** |  | [optional] [default to undefined]
**access_date** | **string** |  | [optional] [default to undefined]
**access_type** | **number** |  | [optional] [default to undefined]
**data_privacy** | **string** |  | [optional] [default to undefined]
**research_outputs** | **object** |  | [optional] [default to undefined]
**data_assets** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { ProjectDetail } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ProjectDetail = {
    id,
    created_at,
    updated_at,
    project_id,
    datasets,
    other_approval_committees,
    data_sensitivity_level,
    legal_basis_for_data_article6,
    duty_of_confidentiality,
    national_data_optout,
    request_frequency,
    dataset_linkage_description,
    data_minimisation,
    data_use_description,
    access_date,
    access_type,
    data_privacy,
    research_outputs,
    data_assets,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
