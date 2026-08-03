# SystemConfig

Model representing system configuration settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the system configuration | [optional] [default to undefined]
**name** | **string** | Name of the configuration setting | [optional] [default to undefined]
**value** | **string** | Value of the configuration setting | [optional] [default to undefined]
**description** | **string** | Description of the configuration setting | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the configuration was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the configuration was last updated | [optional] [default to undefined]

## Example

```typescript
import { SystemConfig } from '@hdruk/safepeopleregistry-api-sdk';

const instance: SystemConfig = {
    id,
    name,
    value,
    description,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
