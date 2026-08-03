# OrganisationHasCharity

Pivot model representing the relationship between organisations and charities

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the organisation-charity relationship | [optional] [default to undefined]
**organisation_id** | **number** | ID of the organisation | [optional] [default to undefined]
**charity_id** | **number** | ID of the charity | [optional] [default to undefined]

## Example

```typescript
import { OrganisationHasCharity } from '@hdruk/safepeopleregistry-api-sdk';

const instance: OrganisationHasCharity = {
    id,
    organisation_id,
    charity_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
