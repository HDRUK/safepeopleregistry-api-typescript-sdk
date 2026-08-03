# RegistryHasAffiliation

Pivot model representing the relationship between registries and affiliations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the registry-affiliation relationship | [optional] [default to undefined]
**registry_id** | **number** | ID of the registry | [optional] [default to undefined]
**affiliation_id** | **number** | ID of the affiliation | [optional] [default to undefined]

## Example

```typescript
import { RegistryHasAffiliation } from '@hdruk/safepeopleregistry-api-sdk';

const instance: RegistryHasAffiliation = {
    id,
    registry_id,
    affiliation_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
