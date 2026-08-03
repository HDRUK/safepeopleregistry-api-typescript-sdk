# UserHasCustodianPermission

Pivot model representing the relationship between users, custodians, and permissions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **number** | ID of the user | [optional] [default to undefined]
**permission_id** | **number** | ID of the permission | [optional] [default to undefined]
**custodian_id** | **number** | ID of the custodian | [optional] [default to undefined]

## Example

```typescript
import { UserHasCustodianPermission } from '@hdruk/safepeopleregistry-api-sdk';

const instance: UserHasCustodianPermission = {
    user_id,
    permission_id,
    custodian_id,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
