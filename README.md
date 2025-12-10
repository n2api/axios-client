## @n2api/axios-client@0.0.1

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
npm install @n2api/axios-client@0.0.1 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *https://api.n2api.io*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ActiveAgentApi* | [**_delete**](docs/ActiveAgentApi.md#_delete) | **DELETE** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | 
*ActiveAgentApi* | [**_delete_0**](docs/ActiveAgentApi.md#_delete_0) | **DELETE** /activeagent/credentials | 
*ActiveAgentApi* | [**create**](docs/ActiveAgentApi.md#create) | **POST** /activeagent/campaigns | 
*ActiveAgentApi* | [**createCustomer**](docs/ActiveAgentApi.md#createcustomer) | **POST** /activeagent/credentials/customer | 
*ActiveAgentApi* | [**create_0**](docs/ActiveAgentApi.md#create_0) | **POST** /activeagent/{resource}/{resourceId}/targeting | 
*ActiveAgentApi* | [**create_1**](docs/ActiveAgentApi.md#create_1) | **POST** /activeagent/adsets | 
*ActiveAgentApi* | [**find**](docs/ActiveAgentApi.md#find) | **GET** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | 
*ActiveAgentApi* | [**findAll**](docs/ActiveAgentApi.md#findall) | **GET** /activeagent/campaigns | 
*ActiveAgentApi* | [**findAll_0**](docs/ActiveAgentApi.md#findall_0) | **GET** /activeagent/adsets | 
*ActiveAgentApi* | [**findAll_1**](docs/ActiveAgentApi.md#findall_1) | **GET** /activeagent/ads | 
*ActiveAgentApi* | [**findAll_2**](docs/ActiveAgentApi.md#findall_2) | **GET** /activeagent/credentials | 
*ActiveAgentApi* | [**findOne**](docs/ActiveAgentApi.md#findone) | **GET** /activeagent/campaigns/{id} | 
*ActiveAgentApi* | [**findOne_0**](docs/ActiveAgentApi.md#findone_0) | **GET** /activeagent/adsets/{id} | 
*ActiveAgentApi* | [**findOne_1**](docs/ActiveAgentApi.md#findone_1) | **GET** /activeagent/ads/{id} | 
*ActiveAgentApi* | [**getReport**](docs/ActiveAgentApi.md#getreport) | **GET** /activeagent/campaigns/{id}/report | 
*ActiveAgentApi* | [**getReport_0**](docs/ActiveAgentApi.md#getreport_0) | **GET** /activeagent/reporting | 
*ActiveAgentApi* | [**rawRequestDelete**](docs/ActiveAgentApi.md#rawrequestdelete) | **DELETE** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawRequestGet**](docs/ActiveAgentApi.md#rawrequestget) | **GET** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawRequestHead**](docs/ActiveAgentApi.md#rawrequesthead) | **HEAD** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawRequestOptions**](docs/ActiveAgentApi.md#rawrequestoptions) | **OPTIONS** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawRequestPatch**](docs/ActiveAgentApi.md#rawrequestpatch) | **PATCH** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawRequestPost**](docs/ActiveAgentApi.md#rawrequestpost) | **POST** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawRequestPut**](docs/ActiveAgentApi.md#rawrequestput) | **PUT** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**remove**](docs/ActiveAgentApi.md#remove) | **DELETE** /activeagent/campaigns/{id} | 
*ActiveAgentApi* | [**remove_0**](docs/ActiveAgentApi.md#remove_0) | **DELETE** /activeagent/adsets/{id} | 
*ActiveAgentApi* | [**sync**](docs/ActiveAgentApi.md#sync) | **PUT** /activeagent/adaccounts | 
*ActiveAgentApi* | [**syncCustomer**](docs/ActiveAgentApi.md#synccustomer) | **PUT** /activeagent/adaccounts/customer | 
*ActiveAgentApi* | [**translate**](docs/ActiveAgentApi.md#translate) | **POST** /activeagent/campaigns/translate | 
*ActiveAgentApi* | [**update**](docs/ActiveAgentApi.md#update) | **PATCH** /activeagent/campaigns/{id} | 
*ActiveAgentApi* | [**updateOrCreate**](docs/ActiveAgentApi.md#updateorcreate) | **PUT** /activeagent/{resource}/{resourceId}/targeting | 
*ActiveAgentApi* | [**update_0**](docs/ActiveAgentApi.md#update_0) | **PATCH** /activeagent/adsets/{id} | 
*ActiveAgentApi* | [**update_1**](docs/ActiveAgentApi.md#update_1) | **PUT** /activeagent/credentials | 
*ActiveAgentApi* | [**update_2**](docs/ActiveAgentApi.md#update_2) | **PUT** /activeagent/{resource}/{resourceId}/settings | 
*AdAccountsApi* | [**findAll**](docs/AdAccountsApi.md#findall) | **GET** /adaccounts | 
*AdSetsApi* | [**getAdsets**](docs/AdSetsApi.md#getadsets) | **GET** /adsets | 
*AdsApi* | [**getAds**](docs/AdsApi.md#getads) | **GET** /ads | 
*AuthenticationApi* | [**createCompanyToken**](docs/AuthenticationApi.md#createcompanytoken) | **POST** /auth/company_token | 
*AuthenticationApi* | [**deleteCompanyToken**](docs/AuthenticationApi.md#deletecompanytoken) | **DELETE** /auth/company_token | 
*AuthenticationApi* | [**getCompanyToken**](docs/AuthenticationApi.md#getcompanytoken) | **GET** /auth/company_token | 
*AuthenticationApi* | [**getHello**](docs/AuthenticationApi.md#gethello) | **GET** /auth/user | 
*AuthenticationApi* | [**getSessionToken**](docs/AuthenticationApi.md#getsessiontoken) | **POST** /auth/session_token | 
*AuthenticationApi* | [**login**](docs/AuthenticationApi.md#login) | **POST** /auth/login | Login
*AuthenticationApi* | [**refresh**](docs/AuthenticationApi.md#refresh) | **POST** /auth/refresh | 
*AuthenticationApi* | [**verifySessionToken**](docs/AuthenticationApi.md#verifysessiontoken) | **POST** /auth/session_token/verify | 
*CampaignsApi* | [**getCampaigns**](docs/CampaignsApi.md#getcampaigns) | **GET** /campaigns | 
*CompaniesApi* | [**getCompany**](docs/CompaniesApi.md#getcompany) | **GET** /companies | 
*CompaniesApi* | [**getRedirectUri**](docs/CompaniesApi.md#getredirecturi) | **GET** /companies/redirect_uri | 
*CompaniesApi* | [**setRedirectUri**](docs/CompaniesApi.md#setredirecturi) | **PUT** /companies/redirect_uri | 
*CustomersApi* | [**createCustomer**](docs/CustomersApi.md#createcustomer) | **POST** /customers | Create customer
*CustomersApi* | [**deleteCustomer**](docs/CustomersApi.md#deletecustomer) | **DELETE** /customers/{id} | Delete customer
*CustomersApi* | [**generateConnectCustomerUrl**](docs/CustomersApi.md#generateconnectcustomerurl) | **GET** /customers/{id}/connect | Generate connect URL for a customer
*CustomersApi* | [**getAllCustomers**](docs/CustomersApi.md#getallcustomers) | **GET** /customers | Get all customers
*CustomersApi* | [**getAllCustomersWithPlatforms**](docs/CustomersApi.md#getallcustomerswithplatforms) | **GET** /customers/platforms | Get all customers with platforms
*CustomersApi* | [**getCustomer**](docs/CustomersApi.md#getcustomer) | **GET** /customers/{id} | Get customer by id
*CustomersApi* | [**getCustomerWithPlatforms**](docs/CustomersApi.md#getcustomerwithplatforms) | **GET** /customers/{id}/platforms | Get customer with platforms
*FacebookApi* | [**createCustomer**](docs/FacebookApi.md#createcustomer) | **POST** /facebook/credentials/customer | 
*FacebookApi* | [**deleteCustomer**](docs/FacebookApi.md#deletecustomer) | **DELETE** /facebook/credentials/{customerId} | 
*FacebookApi* | [**findAll**](docs/FacebookApi.md#findall) | **GET** /facebook/credentials | 
*FacebookApi* | [**findAll_0**](docs/FacebookApi.md#findall_0) | **GET** /facebook/campaigns | 
*FacebookApi* | [**findAll_1**](docs/FacebookApi.md#findall_1) | **GET** /facebook/adsets | 
*FacebookApi* | [**findAll_2**](docs/FacebookApi.md#findall_2) | **GET** /facebook/adaccounts | 
*FacebookApi* | [**findOne**](docs/FacebookApi.md#findone) | **GET** /facebook/adsets/{id} | 
*FacebookApi* | [**getAccessToken**](docs/FacebookApi.md#getaccesstoken) | **POST** /facebook/auth | 
*FacebookApi* | [**isConnected**](docs/FacebookApi.md#isconnected) | **GET** /facebook/credentials/isConnected | 
*FacebookApi* | [**rawRequestDelete**](docs/FacebookApi.md#rawrequestdelete) | **DELETE** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawRequestGet**](docs/FacebookApi.md#rawrequestget) | **GET** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawRequestHead**](docs/FacebookApi.md#rawrequesthead) | **HEAD** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawRequestOptions**](docs/FacebookApi.md#rawrequestoptions) | **OPTIONS** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawRequestPatch**](docs/FacebookApi.md#rawrequestpatch) | **PATCH** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawRequestPost**](docs/FacebookApi.md#rawrequestpost) | **POST** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawRequestPut**](docs/FacebookApi.md#rawrequestput) | **PUT** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**remove**](docs/FacebookApi.md#remove) | **DELETE** /facebook/adsets/{id} | 
*FacebookApi* | [**syncCustomer**](docs/FacebookApi.md#synccustomer) | **PUT** /facebook/adaccounts/customer | 
*FacebookApi* | [**update**](docs/FacebookApi.md#update) | **PATCH** /facebook/adsets/{id} | 
*GoogleAdsApi* | [**create**](docs/GoogleAdsApi.md#create) | **POST** /googleads/campaigns | 
*GoogleAdsApi* | [**createCustomer**](docs/GoogleAdsApi.md#createcustomer) | **POST** /googleads/credentials/customer | 
*GoogleAdsApi* | [**create_0**](docs/GoogleAdsApi.md#create_0) | **POST** /googleads/ads | 
*GoogleAdsApi* | [**create_1**](docs/GoogleAdsApi.md#create_1) | **POST** /googleads/adsets | 
*GoogleAdsApi* | [**deleteCustomerCredentials**](docs/GoogleAdsApi.md#deletecustomercredentials) | **DELETE** /googleads/{customerId}/credentials | 
*GoogleAdsApi* | [**findAll**](docs/GoogleAdsApi.md#findall) | **GET** /googleads/credentials | 
*GoogleAdsApi* | [**findAll_0**](docs/GoogleAdsApi.md#findall_0) | **GET** /googleads/campaigns | 
*GoogleAdsApi* | [**findAll_1**](docs/GoogleAdsApi.md#findall_1) | **GET** /googleads/ads | 
*GoogleAdsApi* | [**findAll_2**](docs/GoogleAdsApi.md#findall_2) | **GET** /googleads/adsets | 
*GoogleAdsApi* | [**findAll_3**](docs/GoogleAdsApi.md#findall_3) | **GET** /googleads/adaccounts | 
*GoogleAdsApi* | [**findOne**](docs/GoogleAdsApi.md#findone) | **GET** /googleads/campaigns/{id} | 
*GoogleAdsApi* | [**findOne_0**](docs/GoogleAdsApi.md#findone_0) | **GET** /googleads/ads/{id} | 
*GoogleAdsApi* | [**findOne_1**](docs/GoogleAdsApi.md#findone_1) | **GET** /googleads/adsets/{id} | 
*GoogleAdsApi* | [**getAccessToken**](docs/GoogleAdsApi.md#getaccesstoken) | **POST** /googleads/auth | 
*GoogleAdsApi* | [**rawRequestDelete**](docs/GoogleAdsApi.md#rawrequestdelete) | **DELETE** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawRequestGet**](docs/GoogleAdsApi.md#rawrequestget) | **GET** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawRequestHead**](docs/GoogleAdsApi.md#rawrequesthead) | **HEAD** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawRequestOptions**](docs/GoogleAdsApi.md#rawrequestoptions) | **OPTIONS** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawRequestPatch**](docs/GoogleAdsApi.md#rawrequestpatch) | **PATCH** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawRequestPost**](docs/GoogleAdsApi.md#rawrequestpost) | **POST** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawRequestPut**](docs/GoogleAdsApi.md#rawrequestput) | **PUT** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**remove**](docs/GoogleAdsApi.md#remove) | **DELETE** /googleads/campaigns/{id} | 
*GoogleAdsApi* | [**remove_0**](docs/GoogleAdsApi.md#remove_0) | **DELETE** /googleads/ads/{id} | 
*GoogleAdsApi* | [**remove_1**](docs/GoogleAdsApi.md#remove_1) | **DELETE** /googleads/adsets/{id} | 
*GoogleAdsApi* | [**syncCustomer**](docs/GoogleAdsApi.md#synccustomer) | **PUT** /googleads/{customerId}/adaccounts | 
*GoogleAdsApi* | [**update**](docs/GoogleAdsApi.md#update) | **PATCH** /googleads/campaigns/{id} | 
*GoogleAdsApi* | [**update_0**](docs/GoogleAdsApi.md#update_0) | **PATCH** /googleads/ads/{id} | 
*GoogleAdsApi* | [**update_1**](docs/GoogleAdsApi.md#update_1) | **PATCH** /googleads/adsets/{id} | 
*LinkedInApi* | [**createCustomer**](docs/LinkedInApi.md#createcustomer) | **POST** /linkedin/credentials/customer | Store LinkedIn credentials for a customer
*LinkedInApi* | [**deleteCustomer**](docs/LinkedInApi.md#deletecustomer) | **DELETE** /linkedin/credentials/{customerId} | Delete LinkedIn credentials for a customer
*LinkedInApi* | [**getAccessToken**](docs/LinkedInApi.md#getaccesstoken) | **POST** /linkedin/auth | Convert LinkedIn auth code
*LinkedInApi* | [**rawRequestDelete**](docs/LinkedInApi.md#rawrequestdelete) | **DELETE** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API
*LinkedInApi* | [**rawRequestGet**](docs/LinkedInApi.md#rawrequestget) | **GET** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API
*LinkedInApi* | [**rawRequestHead**](docs/LinkedInApi.md#rawrequesthead) | **HEAD** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API
*LinkedInApi* | [**rawRequestOptions**](docs/LinkedInApi.md#rawrequestoptions) | **OPTIONS** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API
*LinkedInApi* | [**rawRequestPatch**](docs/LinkedInApi.md#rawrequestpatch) | **PATCH** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API
*LinkedInApi* | [**rawRequestPost**](docs/LinkedInApi.md#rawrequestpost) | **POST** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API
*LinkedInApi* | [**rawRequestPut**](docs/LinkedInApi.md#rawrequestput) | **PUT** /linkedin/{customerId}/raw/{externalPath} | Proxy raw requests to the LinkedIn API
*PinterestApi* | [**createCustomer**](docs/PinterestApi.md#createcustomer) | **POST** /pinterest/credentials/customer | Store Pinterest credentials for a customer
*PinterestApi* | [**deleteCustomerCredentials**](docs/PinterestApi.md#deletecustomercredentials) | **DELETE** /pinterest/credentials/{customerId} | Delete Pinterest credentials for a customer
*PinterestApi* | [**getAccessToken**](docs/PinterestApi.md#getaccesstoken) | **POST** /pinterest/auth | Convert Pinterest auth code
*PinterestApi* | [**rawRequestDelete**](docs/PinterestApi.md#rawrequestdelete) | **DELETE** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequestGet**](docs/PinterestApi.md#rawrequestget) | **GET** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequestHead**](docs/PinterestApi.md#rawrequesthead) | **HEAD** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequestOptions**](docs/PinterestApi.md#rawrequestoptions) | **OPTIONS** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequestPatch**](docs/PinterestApi.md#rawrequestpatch) | **PATCH** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequestPost**](docs/PinterestApi.md#rawrequestpost) | **POST** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequestPut**](docs/PinterestApi.md#rawrequestput) | **PUT** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*ReportingApi* | [**getReport**](docs/ReportingApi.md#getreport) | **GET** /reporting | 
*TheTradeDeskApi* | [**create**](docs/TheTradeDeskApi.md#create) | **POST** /thetradedesk/credentials/customer | Login to The Trade Desk
*TheTradeDeskApi* | [**rawRequestDelete**](docs/TheTradeDeskApi.md#rawrequestdelete) | **DELETE** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequestGet**](docs/TheTradeDeskApi.md#rawrequestget) | **GET** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequestHead**](docs/TheTradeDeskApi.md#rawrequesthead) | **HEAD** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequestOptions**](docs/TheTradeDeskApi.md#rawrequestoptions) | **OPTIONS** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequestPatch**](docs/TheTradeDeskApi.md#rawrequestpatch) | **PATCH** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequestPost**](docs/TheTradeDeskApi.md#rawrequestpost) | **POST** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequestPut**](docs/TheTradeDeskApi.md#rawrequestput) | **PUT** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API


### Documentation For Models

 - [ActiveAgentCreateCredentialDto](docs/ActiveAgentCreateCredentialDto.md)
 - [ChannelKind](docs/ChannelKind.md)
 - [CreateAuthDto](docs/CreateAuthDto.md)
 - [CreateCustomerDto](docs/CreateCustomerDto.md)
 - [CreateFacebookAuthDto](docs/CreateFacebookAuthDto.md)
 - [CreateGoogleAdsAuthDto](docs/CreateGoogleAdsAuthDto.md)
 - [CreatePinterestAuthDto](docs/CreatePinterestAuthDto.md)
 - [CreateSettingDto](docs/CreateSettingDto.md)
 - [CreateSettingDtoSettingsInner](docs/CreateSettingDtoSettingsInner.md)
 - [CreateTargetingDto](docs/CreateTargetingDto.md)
 - [CreateTargetingDtoTargetingsInner](docs/CreateTargetingDtoTargetingsInner.md)
 - [CustomerDto](docs/CustomerDto.md)
 - [CustomerWithPlatformsDto](docs/CustomerWithPlatformsDto.md)
 - [FacebookCreateCredentialDto](docs/FacebookCreateCredentialDto.md)
 - [GoogleAdsCreateCredentialDto](docs/GoogleAdsCreateCredentialDto.md)
 - [LinkedInCreateCredentialDto](docs/LinkedInCreateCredentialDto.md)
 - [LoginDto](docs/LoginDto.md)
 - [PinterestCreateCredentialDto](docs/PinterestCreateCredentialDto.md)
 - [PlatformName](docs/PlatformName.md)
 - [RedirectUriDTO](docs/RedirectUriDTO.md)
 - [ResourceKind](docs/ResourceKind.md)
 - [SessionTokenDto](docs/SessionTokenDto.md)
 - [SessionTokenVerifyDto](docs/SessionTokenVerifyDto.md)
 - [Status](docs/Status.md)
 - [TheTradeDeskCreateCredentialsDto](docs/TheTradeDeskCreateCredentialsDto.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="bearerAuth"></a>
### bearerAuth

- **Type**: Bearer authentication (JWT)

