# Organisation

Organisation model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **number** | Model primary key | [optional] [default to undefined]
**created_at** | **string** |  | [optional] [default to undefined]
**updated_at** | **string** |  | [optional] [default to undefined]
**organisation_name** | **string** |  | [optional] [default to undefined]
**address_1** | **string** |  | [optional] [default to undefined]
**address_2** | **string** |  | [optional] [default to undefined]
**town** | **string** |  | [optional] [default to undefined]
**county** | **string** |  | [optional] [default to undefined]
**country** | **string** |  | [optional] [default to undefined]
**postcode** | **string** |  | [optional] [default to undefined]
**lead_applicant_organisation_name** | **string** |  | [optional] [default to undefined]
**lead_applicant_email** | **string** |  | [optional] [default to undefined]
**organisation_unique_id** | **string** |  | [optional] [default to undefined]
**applicant_names** | **string** |  | [optional] [default to undefined]
**funders_and_sponsors** | **string** |  | [optional] [default to undefined]
**sub_license_arrangements** | **string** |  | [optional] [default to undefined]
**verified** | **boolean** |  | [optional] [default to undefined]
**dsptk_ods_code** | **string** |  | [optional] [default to undefined]
**dsptk_certified** | **boolean** |  | [optional] [default to undefined]
**dsptk_expiry_date** | **string** |  | [optional] [default to undefined]
**iso_27001_certified** | **boolean** |  | [optional] [default to undefined]
**iso_27001_certification_num** | **string** |  | [optional] [default to undefined]
**iso_expiry_date** | **string** |  | [optional] [default to undefined]
**ce_certified** | **boolean** |  | [optional] [default to undefined]
**ce_certification_num** | **string** |  | [optional] [default to undefined]
**ce_expiry_date** | **string** |  | [optional] [default to undefined]
**ce_plus_certified** | **boolean** |  | [optional] [default to undefined]
**ce_plus_certification_num** | **string** |  | [optional] [default to undefined]
**ce_plus_expiry_date** | **string** |  | [optional] [default to undefined]
**idvt_result** | **number** |  | [optional] [default to undefined]
**idvt_result_perc** | **number** |  | [optional] [default to undefined]
**idvt_errors** | **string** |  | [optional] [default to undefined]
**idvt_completed_at** | **string** |  | [optional] [default to undefined]
**companies_house_no** | **string** |  | [optional] [default to undefined]
**sector_id** | **number** |  | [optional] [default to undefined]
**ror_id** | **string** | ROR.org identification for Research Organisations | [optional] [default to undefined]
**website** | **string** |  | [optional] [default to undefined]
**smb_status** | **boolean** | Declaration of small/medium business | [optional] [default to undefined]
**organisation_size** | **number** | Organisation size. Integer denotes list index rather than absolute value | [optional] [default to undefined]
**unclaimed** | **boolean** | Unclaimed | [optional] [default to undefined]
**system_approved** | **boolean** | Whether this Organisation has been approved to use the system or not | [optional] [default to undefined]
**ods_id** | **string** |  | [optional] [default to undefined]
**dsptk_status** | **string** |  | [optional] [default to undefined]
**dsptk_date_last_published** | **string** |  | [optional] [default to undefined]
**ico_registration_id** | **string** |  | [optional] [default to undefined]
**ico_date_registered** | **string** |  | [optional] [default to undefined]
**ico_expiry_date** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { Organisation } from '@hdruk/safepeopleregistry-api-sdk';

const instance: Organisation = {
    id,
    created_at,
    updated_at,
    organisation_name,
    address_1,
    address_2,
    town,
    county,
    country,
    postcode,
    lead_applicant_organisation_name,
    lead_applicant_email,
    organisation_unique_id,
    applicant_names,
    funders_and_sponsors,
    sub_license_arrangements,
    verified,
    dsptk_ods_code,
    dsptk_certified,
    dsptk_expiry_date,
    iso_27001_certified,
    iso_27001_certification_num,
    iso_expiry_date,
    ce_certified,
    ce_certification_num,
    ce_expiry_date,
    ce_plus_certified,
    ce_plus_certification_num,
    ce_plus_expiry_date,
    idvt_result,
    idvt_result_perc,
    idvt_errors,
    idvt_completed_at,
    companies_house_no,
    sector_id,
    ror_id,
    website,
    smb_status,
    organisation_size,
    unclaimed,
    system_approved,
    ods_id,
    dsptk_status,
    dsptk_date_last_published,
    ico_registration_id,
    ico_date_registered,
    ico_expiry_date,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
