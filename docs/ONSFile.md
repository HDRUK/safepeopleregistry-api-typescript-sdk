# ONSFile

Model representing ONS files

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the ONS file | [optional] [default to undefined]
**name** | **string** | Name of the ONS file | [optional] [default to undefined]
**path** | **string** | Path to the ONS file | [optional] [default to undefined]
**status** | **string** | Status of the ONS file | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the ONS file was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the ONS file was last updated | [optional] [default to undefined]

## Example

```typescript
import { ONSFile } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ONSFile = {
    id,
    name,
    path,
    status,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
