## @hdruk/safepeopleregistry-api-sdk@1.36.0

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install @hdruk/safepeopleregistry-api-sdk@1.36.0 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CustodianUserApi* | [**custodianUserBulkStore**](docs/CustodianUserApi.md#custodianuserbulkstore) | **POST** /api/v1/custodian_users/bulk | Create multiple CustodianUser entries
*FeatureApi* | [**featureIndex**](docs/FeatureApi.md#featureindex) | **GET** /api/v1/features | Feature@index
*ProjectUsersApi* | [**projectUsersBulkInviteProjectUsers**](docs/ProjectUsersApi.md#projectusersbulkinviteprojectusers) | **POST** /api/v1/project_users/bulk | Bulk invite Project Users
*QueryApi* | [**queryQuery**](docs/QueryApi.md#queryquery) | **POST** /api/v1/query | Query@query
*VendorWebhookReceiverApi* | [**vendorWebhookReceiverReceive**](docs/VendorWebhookReceiverApi.md#vendorwebhookreceiverreceive) | **POST** /api/v1/webhooks/{provider} | Receive a webhook callback from a vendor


### Documentation For Models

 - [Accreditation](docs/Accreditation.md)
 - [ActionLog](docs/ActionLog.md)
 - [Affiliation](docs/Affiliation.md)
 - [Charity](docs/Charity.md)
 - [Custodian](docs/Custodian.md)
 - [CustodianHasProjectOrganisation](docs/CustodianHasProjectOrganisation.md)
 - [CustodianHasProjectUser](docs/CustodianHasProjectUser.md)
 - [CustodianModelConfig](docs/CustodianModelConfig.md)
 - [CustodianUser](docs/CustodianUser.md)
 - [CustodianUserBulkStore201Response](docs/CustodianUserBulkStore201Response.md)
 - [CustodianUserBulkStore500Response](docs/CustodianUserBulkStore500Response.md)
 - [CustodianUserBulkStoreRequest](docs/CustodianUserBulkStoreRequest.md)
 - [CustodianUserBulkStoreRequestUsersInner](docs/CustodianUserBulkStoreRequestUsersInner.md)
 - [CustodianUserHasPermission](docs/CustodianUserHasPermission.md)
 - [CustodianWebhookReceiver](docs/CustodianWebhookReceiver.md)
 - [DebugLog](docs/DebugLog.md)
 - [DecisionModel](docs/DecisionModel.md)
 - [DecisionModelType](docs/DecisionModelType.md)
 - [Department](docs/Department.md)
 - [Education](docs/Education.md)
 - [Endorsement](docs/Endorsement.md)
 - [Experience](docs/Experience.md)
 - [FeatureIndex200Response](docs/FeatureIndex200Response.md)
 - [FeatureIndex200ResponseData](docs/FeatureIndex200ResponseData.md)
 - [FeatureIndex404Response](docs/FeatureIndex404Response.md)
 - [History](docs/History.md)
 - [IDVTPlugin](docs/IDVTPlugin.md)
 - [Identity](docs/Identity.md)
 - [Infringement](docs/Infringement.md)
 - [InfringementHasResolution](docs/InfringementHasResolution.md)
 - [ModelFile](docs/ModelFile.md)
 - [ModelState](docs/ModelState.md)
 - [ONSFile](docs/ONSFile.md)
 - [Organisation](docs/Organisation.md)
 - [OrganisationHasCharity](docs/OrganisationHasCharity.md)
 - [OrganisationHasCustodianPermission](docs/OrganisationHasCustodianPermission.md)
 - [OrganisationHasDepartment](docs/OrganisationHasDepartment.md)
 - [OrganisationHasFile](docs/OrganisationHasFile.md)
 - [OrganisationHasSubsidiary](docs/OrganisationHasSubsidiary.md)
 - [PendingInvite](docs/PendingInvite.md)
 - [Permission](docs/Permission.md)
 - [ProfessionalRegistration](docs/ProfessionalRegistration.md)
 - [Project](docs/Project.md)
 - [ProjectDetail](docs/ProjectDetail.md)
 - [ProjectHasCustodian](docs/ProjectHasCustodian.md)
 - [ProjectHasOrganisation](docs/ProjectHasOrganisation.md)
 - [ProjectHasRole](docs/ProjectHasRole.md)
 - [ProjectHasUser](docs/ProjectHasUser.md)
 - [ProjectRole](docs/ProjectRole.md)
 - [ProjectUsersBulkInviteProjectUsersRequest](docs/ProjectUsersBulkInviteProjectUsersRequest.md)
 - [ProjectUsersBulkInviteProjectUsersRequestUsersInner](docs/ProjectUsersBulkInviteProjectUsersRequestUsersInner.md)
 - [QueryQuery200Response](docs/QueryQuery200Response.md)
 - [QueryQuery200ResponseData](docs/QueryQuery200ResponseData.md)
 - [QueryQuery200ResponseDataProjectsInner](docs/QueryQuery200ResponseDataProjectsInner.md)
 - [QueryQuery200ResponseDataRegistry](docs/QueryQuery200ResponseDataRegistry.md)
 - [QueryQuery200ResponseDataRegistryAllOfHistoryInner](docs/QueryQuery200ResponseDataRegistryAllOfHistoryInner.md)
 - [QueryQuery200ResponseDataUser](docs/QueryQuery200ResponseDataUser.md)
 - [QueryQuery401Response](docs/QueryQuery401Response.md)
 - [QueryQueryRequest](docs/QueryQueryRequest.md)
 - [Registry](docs/Registry.md)
 - [RegistryHasAccreditation](docs/RegistryHasAccreditation.md)
 - [RegistryHasAffiliation](docs/RegistryHasAffiliation.md)
 - [RegistryHasEducation](docs/RegistryHasEducation.md)
 - [RegistryHasFile](docs/RegistryHasFile.md)
 - [RegistryHasHistory](docs/RegistryHasHistory.md)
 - [RegistryHasProfessionalRegistration](docs/RegistryHasProfessionalRegistration.md)
 - [RegistryHasTraining](docs/RegistryHasTraining.md)
 - [Resolution](docs/Resolution.md)
 - [Sector](docs/Sector.md)
 - [SsoTenant](docs/SsoTenant.md)
 - [SsoTenantDomain](docs/SsoTenantDomain.md)
 - [State](docs/State.md)
 - [Subsidiary](docs/Subsidiary.md)
 - [SystemConfig](docs/SystemConfig.md)
 - [Training](docs/Training.md)
 - [TrainingHasFile](docs/TrainingHasFile.md)
 - [UksaLiveFeed](docs/UksaLiveFeed.md)
 - [User](docs/User.md)
 - [UserHasCustodianPermission](docs/UserHasCustodianPermission.md)
 - [UserHasDepartments](docs/UserHasDepartments.md)
 - [ValidationCheck](docs/ValidationCheck.md)
 - [ValidationLog](docs/ValidationLog.md)
 - [ValidationLogComment](docs/ValidationLogComment.md)
 - [VendorWebhookReceiverReceive200Response](docs/VendorWebhookReceiverReceive200Response.md)
 - [VendorWebhookReceiverReceive400Response](docs/VendorWebhookReceiverReceive400Response.md)
 - [VendorWebhookReceiverReceive500Response](docs/VendorWebhookReceiverReceive500Response.md)
 - [WebhookEventTrigger](docs/WebhookEventTrigger.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization

Endpoints do not require authorization.

