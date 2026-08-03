# DebugLog

Model representing debug logs

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the debug log | [optional] [default to undefined]
**_class** | **string** | Class name where the log was generated | [optional] [default to undefined]
**log** | **string** | Log message | [optional] [default to undefined]
**created_at** | **string** | Timestamp when the log was created | [optional] [default to undefined]
**updated_at** | **string** | Timestamp when the log was last updated | [optional] [default to undefined]

## Example

```typescript
import { DebugLog } from '@hdruk/safepeopleregistry-api-sdk';

const instance: DebugLog = {
    id,
    _class,
    log,
    created_at,
    updated_at,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
