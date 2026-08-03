# Resolution

Model representing resolutions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the resolution | [optional] [default to undefined]
**comment** | **string** | Comment associated with the resolution | [optional] [default to undefined]
**custodian_by** | **number** | ID of the custodian who resolved the issue | [optional] [default to undefined]
**registry_id** | **number** | ID of the registry associated with the resolution | [optional] [default to undefined]
**resolved** | **boolean** | Indicates whether the resolution is resolved | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the resolution was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the resolution was last updated | [optional] [default to undefined]

## Example

```typescript
import { Resolution } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Resolution = {
    id,
    comment,
    custodian_by,
    registry_id,
    resolved,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
