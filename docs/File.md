# ModelFile

Model representing files

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the file | [optional] [default to undefined]
**name** | **string** | Name of the file | [optional] [default to undefined]
**type** | **string** | Type of the file | [optional] [default to undefined]
**path** | **string** | Path to the file | [optional] [default to undefined]
**status** | **string** | Status of the file | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the file was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the file was last updated | [optional] [default to undefined]

## Example

```typescript
import { ModelFile } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ModelFile = {
    id,
    name,
    type,
    path,
    status,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
