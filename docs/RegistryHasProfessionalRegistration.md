# RegistryHasProfessionalRegistration

Pivot model representing the relationship between registries and professional registrations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the registry-professional registration relationship | [optional] [default to undefined]
**registry_id** | **number** | ID of the registry | [optional] [default to undefined]
**professional_registration_id** | **number** | ID of the professional registration | [optional] [default to undefined]

## Example

```typescript
import { RegistryHasProfessionalRegistration } from '@hdruk/safepeopleregistry-api-sdk';

const instance: RegistryHasProfessionalRegistration = {
    id,
    registry_id,
    professional_registration_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
