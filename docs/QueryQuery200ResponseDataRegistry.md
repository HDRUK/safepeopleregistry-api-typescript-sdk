# QueryQuery200ResponseDataRegistry

The matched Registry record

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** |  | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**deleted_at** | **string** |  | [optional] [default to undefined]
**digi_ident** | **string** |  | [optional] [default to undefined]
**dl_ident** | **string** |  | [optional] [default to undefined]
**pp_ident** | **string** |  | [optional] [default to undefined]
**verified** | **number** |  | [optional] [default to undefined]
**training** | [**Array&lt;Training&gt;**](Training.md) | Training records linked to the registry | [optional] [default to undefined]
**history** | [**Array&lt;QueryQuery200ResponseDataRegistryAllOfHistoryInner&gt;**](QueryQuery200ResponseDataRegistryAllOfHistoryInner.md) | History records linked to the registry, each with its related affiliation and project | [optional] [default to undefined]

## Example

```typescript
import { QueryQuery200ResponseDataRegistry } from '@hdruk/safepeopleregistry-api-sdk';

const instance: QueryQuery200ResponseDataRegistry = {
    id,
    created_at,
    updated_at,
    deleted_at,
    digi_ident,
    dl_ident,
    pp_ident,
    verified,
    training,
    history,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
