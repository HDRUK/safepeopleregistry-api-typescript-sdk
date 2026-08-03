# Charity

Charity model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Unique identifier for the charity | [optional] [default to undefined]
**registration_id** | **string** | Registration ID of the charity | [optional] [default to undefined]
**name** | **string** | Name of the charity | [optional] [default to undefined]
**website** | **string** | Website URL of the charity | [optional] [default to undefined]
**address_1** | **string** | First line of the charity\&#39;s address | [optional] [default to undefined]
**address_2** | **string** | Second line of the charity\&#39;s address | [optional] [default to undefined]
**town** | **string** | Town where the charity is located | [optional] [default to undefined]
**county** | **string** | County where the charity is located | [optional] [default to undefined]
**country** | **string** | Country where the charity is located | [optional] [default to undefined]
**postcode** | **string** | Postcode of the charity\&#39;s address | [optional] [default to undefined]

## Example

```typescript
import { Charity } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Charity = {
    id,
    registration_id,
    name,
    website,
    address_1,
    address_2,
    town,
    county,
    country,
    postcode,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
