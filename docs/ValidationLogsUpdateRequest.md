# ValidationLogsUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**complete** | **boolean** | Mark the validation log as complete | [optional] [default to undefined]
**incomplete** | **boolean** | Mark the validation log as incomplete | [optional] [default to undefined]
**pass** | **boolean** | Mark the validation log as passed | [optional] [default to undefined]
**fail** | **boolean** | Mark the validation log as failed | [optional] [default to undefined]
**enable** | **boolean** | Mark the validation log as enabled | [optional] [default to undefined]
**disable** | **boolean** | Mark the validation log as disabled | [optional] [default to undefined]

## Example

```typescript
import { ValidationLogsUpdateRequest } from '@hdruk/safepeopleregistry-api-sdk';

const instance: ValidationLogsUpdateRequest = {
    complete,
    incomplete,
    pass,
    fail,
    enable,
    disable,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
