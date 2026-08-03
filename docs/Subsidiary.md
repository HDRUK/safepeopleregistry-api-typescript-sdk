# Subsidiary

Model representing subsidiaries

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the subsidiary | [optional] [default to undefined]
**name** | **string** | Name of the subsidiary | [optional] [default to undefined]
**address_1** | **string** | Primary address line of the subsidiary | [optional] [default to undefined]
**address_2** | **string** | Secondary address line of the subsidiary | [optional] [default to undefined]
**town** | **string** | Town where the subsidiary is located | [optional] [default to undefined]
**county** | **string** | County where the subsidiary is located | [optional] [default to undefined]
**country** | **string** | Country where the subsidiary is located | [optional] [default to undefined]
**postcode** | **string** | Postcode of the subsidiary | [optional] [default to undefined]
**website** | **string** | Website of the subsidiary | [optional] [default to undefined]
**is_parent** | **number** | Indicates if the subsidiary is a parent company | [optional] [default to undefined]

## Example

```typescript
import { Subsidiary } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Subsidiary = {
    id,
    name,
    address_1,
    address_2,
    town,
    county,
    country,
    postcode,
    website,
    is_parent,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
