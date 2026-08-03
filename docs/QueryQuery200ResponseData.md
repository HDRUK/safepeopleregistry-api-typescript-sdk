# QueryQuery200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user** | [**QueryQuery200ResponseDataUser**](QueryQuery200ResponseDataUser.md) |  | [optional] [default to undefined]
**registry** | [**QueryQuery200ResponseDataRegistry**](QueryQuery200ResponseDataRegistry.md) |  | [optional] [default to undefined]
**projects** | [**Array&lt;QueryQuery200ResponseDataProjectsInner&gt;**](QueryQuery200ResponseDataProjectsInner.md) | Projects the queried user is linked to, scoped to the requesting custodian | [optional] [default to undefined]

## Example

```typescript
import { QueryQuery200ResponseData } from '@hdruk/safepeopleregistry-api-sdk';

const instance: QueryQuery200ResponseData = {
    user,
    registry,
    projects,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
