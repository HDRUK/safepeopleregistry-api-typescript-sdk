# Project

Project model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]
**unique_id** | **string** |  | [optional] [default to undefined]
**lay_summary** | **string** |  | [optional] [default to undefined]
**public_benefit** | **string** | A unique identifier for Custodian\&#39;s within SOURSD | [optional] [default to undefined]
**request_category_type** | **string** |  | [optional] [default to undefined]
**technical_summary** | **string** |  | [optional] [default to undefined]
**other_approval_commitees** | **string** |  | [optional] [default to undefined]
**start_date** | **string** |  | [optional] [default to undefined]
**end_date** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Project } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Project = {
    id,
    title,
    unique_id,
    lay_summary,
    public_benefit,
    request_category_type,
    technical_summary,
    other_approval_commitees,
    start_date,
    end_date,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
