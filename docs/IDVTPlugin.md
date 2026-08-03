# IDVTPlugin

Model representing IDVT plugins

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the IDVT plugin | [optional] [default to undefined]
**_function** | **string** | Function name of the plugin | [optional] [default to undefined]
**args** | **string** | Arguments passed to the plugin function | [optional] [default to undefined]
**config** | **string** | Configuration settings for the plugin | [optional] [default to undefined]
**enabled** | **number** | Indicates whether the plugin is enabled (1 for enabled, 0 for disabled) | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the plugin was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the plugin was last updated | [optional] [default to undefined]

## Example

```typescript
import { IDVTPlugin } from '@hdruk/safepeopleregistry-api-sdk';

const instance: IDVTPlugin = {
    id,
    _function,
    args,
    config,
    enabled,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
