# Permission

Model representing permissions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the permission | [optional] [default to undefined]
**name** | **string** | Name of the permission | [optional] [default to undefined]
**enabled** | **boolean** | Indicates whether the permission is enabled | [optional] [default to undefined]
**description** | **string** | Description of the permission | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the permission was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the permission was last updated | [optional] [default to undefined]

## Example

```typescript
import { Permission } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Permission = {
    id,
    name,
    enabled,
    description,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
