# Education

Model representing education records

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the education record | [optional] [default to undefined]
**title** | **string** | Title of the education qualification | [optional] [default to undefined]
**from** | **string** | Start date of the education qualification | [optional] [default to undefined]
**to** | **string** | End date of the education qualification | [optional] [default to undefined]
**institute_name** | **string** | Name of the educational institute | [optional] [default to undefined]
**institute_address** | **string** | Address of the educational institute | [optional] [default to undefined]
**institute_identifier** | **string** | Identifier for the educational institute | [optional] [default to undefined]
**source** | **string** | Source of the education record | [optional] [default to undefined]
**registry_id** | **number** | ID of the registry associated with the education record | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the education record was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the education record was last updated | [optional] [default to undefined]

## Example

```typescript
import { Education } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Education = {
    id,
    title,
    from,
    to,
    institute_name,
    institute_address,
    institute_identifier,
    source,
    registry_id,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
