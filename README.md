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
*ActiveAgentApi* | [**adAccountsControllerSyncCustomerQ7yxiw**](docs/ActiveAgentApi.md#adaccountscontrollersynccustomerq7yxiw) | **PUT** /activeagent/adaccounts/customer | 
*ActiveAgentApi* | [**adAccountsControllerSyncR5ln7z**](docs/ActiveAgentApi.md#adaccountscontrollersyncr5ln7z) | **PUT** /activeagent/adaccounts | 
*ActiveAgentApi* | [**adsControllerFindAllV0i00i**](docs/ActiveAgentApi.md#adscontrollerfindallv0i00i) | **GET** /activeagent/ads | 
*ActiveAgentApi* | [**adsControllerFindOneKx2rz2**](docs/ActiveAgentApi.md#adscontrollerfindonekx2rz2) | **GET** /activeagent/ads/{id} | 
*ActiveAgentApi* | [**adsetsControllerCreate7ajntd**](docs/ActiveAgentApi.md#adsetscontrollercreate7ajntd) | **POST** /activeagent/adsets | 
*ActiveAgentApi* | [**adsetsControllerFindAll48b5vs**](docs/ActiveAgentApi.md#adsetscontrollerfindall48b5vs) | **GET** /activeagent/adsets | 
*ActiveAgentApi* | [**adsetsControllerFindOneFfcces**](docs/ActiveAgentApi.md#adsetscontrollerfindoneffcces) | **GET** /activeagent/adsets/{id} | 
*ActiveAgentApi* | [**adsetsControllerRemoveJnaag7**](docs/ActiveAgentApi.md#adsetscontrollerremovejnaag7) | **DELETE** /activeagent/adsets/{id} | 
*ActiveAgentApi* | [**adsetsControllerUpdate31j4du**](docs/ActiveAgentApi.md#adsetscontrollerupdate31j4du) | **PATCH** /activeagent/adsets/{id} | 
*ActiveAgentApi* | [**campaignsControllerCreateLsx4bk**](docs/ActiveAgentApi.md#campaignscontrollercreatelsx4bk) | **POST** /activeagent/campaigns | 
*ActiveAgentApi* | [**campaignsControllerFindAllVkjjqn**](docs/ActiveAgentApi.md#campaignscontrollerfindallvkjjqn) | **GET** /activeagent/campaigns | 
*ActiveAgentApi* | [**campaignsControllerFindOne32heet**](docs/ActiveAgentApi.md#campaignscontrollerfindone32heet) | **GET** /activeagent/campaigns/{id} | 
*ActiveAgentApi* | [**campaignsControllerGetReport11en29**](docs/ActiveAgentApi.md#campaignscontrollergetreport11en29) | **GET** /activeagent/campaigns/{id}/report | 
*ActiveAgentApi* | [**campaignsControllerRemoveWx2dfy**](docs/ActiveAgentApi.md#campaignscontrollerremovewx2dfy) | **DELETE** /activeagent/campaigns/{id} | 
*ActiveAgentApi* | [**campaignsControllerTranslateEcvpl4**](docs/ActiveAgentApi.md#campaignscontrollertranslateecvpl4) | **POST** /activeagent/campaigns/translate | 
*ActiveAgentApi* | [**campaignsControllerUpdate058yv3**](docs/ActiveAgentApi.md#campaignscontrollerupdate058yv3) | **PATCH** /activeagent/campaigns/{id} | 
*ActiveAgentApi* | [**credentialsControllerCreateCustomer6ix19k**](docs/ActiveAgentApi.md#credentialscontrollercreatecustomer6ix19k) | **POST** /activeagent/credentials/customer | 
*ActiveAgentApi* | [**credentialsControllerDeleteLt023k**](docs/ActiveAgentApi.md#credentialscontrollerdeletelt023k) | **DELETE** /activeagent/credentials | 
*ActiveAgentApi* | [**credentialsControllerFindAllHu0kra**](docs/ActiveAgentApi.md#credentialscontrollerfindallhu0kra) | **GET** /activeagent/credentials | 
*ActiveAgentApi* | [**credentialsControllerUpdateU7kaen**](docs/ActiveAgentApi.md#credentialscontrollerupdateu7kaen) | **PUT** /activeagent/credentials | 
*ActiveAgentApi* | [**rawControllerRawRequest2jfj97Post**](docs/ActiveAgentApi.md#rawcontrollerrawrequest2jfj97post) | **POST** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawControllerRawRequest5ryooeGet**](docs/ActiveAgentApi.md#rawcontrollerrawrequest5ryooeget) | **GET** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawControllerRawRequest7bmyr4Patch**](docs/ActiveAgentApi.md#rawcontrollerrawrequest7bmyr4patch) | **PATCH** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawControllerRawRequest7qnyhrHead**](docs/ActiveAgentApi.md#rawcontrollerrawrequest7qnyhrhead) | **HEAD** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawControllerRawRequestGpk4z6Put**](docs/ActiveAgentApi.md#rawcontrollerrawrequestgpk4z6put) | **PUT** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawControllerRawRequestO6zyiqDelete**](docs/ActiveAgentApi.md#rawcontrollerrawrequesto6zyiqdelete) | **DELETE** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**rawControllerRawRequestT080myOptions**](docs/ActiveAgentApi.md#rawcontrollerrawrequestt080myoptions) | **OPTIONS** /activeagent/{customerId}/raw/{externalPath} | 
*ActiveAgentApi* | [**reportingControllerGetReportOj3kae**](docs/ActiveAgentApi.md#reportingcontrollergetreportoj3kae) | **GET** /activeagent/reporting | 
*ActiveAgentApi* | [**settingsControllerUpdate6xv72v**](docs/ActiveAgentApi.md#settingscontrollerupdate6xv72v) | **PUT** /activeagent/{resource}/{resourceId}/settings | 
*ActiveAgentApi* | [**targetingControllerCreate36thcg**](docs/ActiveAgentApi.md#targetingcontrollercreate36thcg) | **POST** /activeagent/{resource}/{resourceId}/targeting | 
*ActiveAgentApi* | [**targetingControllerDelete3swtka**](docs/ActiveAgentApi.md#targetingcontrollerdelete3swtka) | **DELETE** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | 
*ActiveAgentApi* | [**targetingControllerFind5148tb**](docs/ActiveAgentApi.md#targetingcontrollerfind5148tb) | **GET** /activeagent/{resource}/{resourceId}/targeting/{targetingKind} | 
*ActiveAgentApi* | [**targetingControllerUpdateOrCreate2h20li**](docs/ActiveAgentApi.md#targetingcontrollerupdateorcreate2h20li) | **PUT** /activeagent/{resource}/{resourceId}/targeting | 
*AdAccountsApi* | [**adAccountsControllerFindAll1f63wu**](docs/AdAccountsApi.md#adaccountscontrollerfindall1f63wu) | **GET** /adaccounts | 
*AdSetsApi* | [**adsetsControllerGetAdsetsJio5sh**](docs/AdSetsApi.md#adsetscontrollergetadsetsjio5sh) | **GET** /adsets | 
*AdsApi* | [**adsControllerGetAds8yhkpx**](docs/AdsApi.md#adscontrollergetads8yhkpx) | **GET** /ads | 
*AuthenticationApi* | [**authControllerCreateCompanyTokenK3gngq**](docs/AuthenticationApi.md#authcontrollercreatecompanytokenk3gngq) | **POST** /auth/company_token | 
*AuthenticationApi* | [**authControllerDeleteCompanyTokenU6zccl**](docs/AuthenticationApi.md#authcontrollerdeletecompanytokenu6zccl) | **DELETE** /auth/company_token | 
*AuthenticationApi* | [**authControllerGetCompanyToken8bpz6u**](docs/AuthenticationApi.md#authcontrollergetcompanytoken8bpz6u) | **GET** /auth/company_token | 
*AuthenticationApi* | [**authControllerGetHelloR0h1ua**](docs/AuthenticationApi.md#authcontrollergethellor0h1ua) | **GET** /auth/user | 
*AuthenticationApi* | [**authControllerGetSessionTokenRbwd43**](docs/AuthenticationApi.md#authcontrollergetsessiontokenrbwd43) | **POST** /auth/session_token | 
*AuthenticationApi* | [**authControllerRefreshHq9r5i**](docs/AuthenticationApi.md#authcontrollerrefreshhq9r5i) | **POST** /auth/refresh | 
*AuthenticationApi* | [**authControllerVerifySessionTokenQkbht6**](docs/AuthenticationApi.md#authcontrollerverifysessiontokenqkbht6) | **POST** /auth/session_token/verify | 
*AuthenticationApi* | [**login**](docs/AuthenticationApi.md#login) | **POST** /auth/login | Login
*CampaignsApi* | [**campaignsControllerGetCampaigns2qcanu**](docs/CampaignsApi.md#campaignscontrollergetcampaigns2qcanu) | **GET** /campaigns | 
*CompaniesApi* | [**companiesControllerGetCompany2lyej4**](docs/CompaniesApi.md#companiescontrollergetcompany2lyej4) | **GET** /companies | 
*CompaniesApi* | [**companiesControllerGetRedirectUriF0i71s**](docs/CompaniesApi.md#companiescontrollergetredirecturif0i71s) | **GET** /companies/redirect_uri | 
*CompaniesApi* | [**companiesControllerSetRedirectUriFcrzml**](docs/CompaniesApi.md#companiescontrollersetredirecturifcrzml) | **PUT** /companies/redirect_uri | 
*CustomersApi* | [**customersControllerCreateCustomer2cjlz2**](docs/CustomersApi.md#customerscontrollercreatecustomer2cjlz2) | **POST** /customers | 
*CustomersApi* | [**customersControllerDeleteCustomer00kwoh**](docs/CustomersApi.md#customerscontrollerdeletecustomer00kwoh) | **DELETE** /customers/{id} | 
*CustomersApi* | [**customersControllerFindAllKggoor**](docs/CustomersApi.md#customerscontrollerfindallkggoor) | **GET** /customers | 
*CustomersApi* | [**customersControllerFindAllWithPlatformsXzeg6k**](docs/CustomersApi.md#customerscontrollerfindallwithplatformsxzeg6k) | **GET** /customers/platforms | 
*CustomersApi* | [**customersControllerFindOneV9u2yc**](docs/CustomersApi.md#customerscontrollerfindonev9u2yc) | **GET** /customers/{id} | 
*CustomersApi* | [**getConnectCustomerUrl**](docs/CustomersApi.md#getconnectcustomerurl) | **GET** /customers/{id}/connect | Generate connect URL for a customer
*FacebookApi* | [**adAccountsControllerFindAll0549lm**](docs/FacebookApi.md#adaccountscontrollerfindall0549lm) | **GET** /facebook/adaccounts | 
*FacebookApi* | [**adAccountsControllerSyncCustomerKpkzo2**](docs/FacebookApi.md#adaccountscontrollersynccustomerkpkzo2) | **PUT** /facebook/adaccounts/customer | 
*FacebookApi* | [**adSetsControllerFindAllGeus8d**](docs/FacebookApi.md#adsetscontrollerfindallgeus8d) | **GET** /facebook/adsets | 
*FacebookApi* | [**adSetsControllerFindOne7d8j59**](docs/FacebookApi.md#adsetscontrollerfindone7d8j59) | **GET** /facebook/adsets/{id} | 
*FacebookApi* | [**adSetsControllerRemoveQpjoni**](docs/FacebookApi.md#adsetscontrollerremoveqpjoni) | **DELETE** /facebook/adsets/{id} | 
*FacebookApi* | [**adSetsControllerUpdate505b7c**](docs/FacebookApi.md#adsetscontrollerupdate505b7c) | **PATCH** /facebook/adsets/{id} | 
*FacebookApi* | [**authControllerGetAccessTokenT41rff**](docs/FacebookApi.md#authcontrollergetaccesstokent41rff) | **POST** /facebook/auth | 
*FacebookApi* | [**campaignsControllerFindAllZ5jbts**](docs/FacebookApi.md#campaignscontrollerfindallz5jbts) | **GET** /facebook/campaigns | 
*FacebookApi* | [**credentialsControllerCreateCustomerLqwsc5**](docs/FacebookApi.md#credentialscontrollercreatecustomerlqwsc5) | **POST** /facebook/credentials/customer | 
*FacebookApi* | [**credentialsControllerDeleteCustomerGkcpsz**](docs/FacebookApi.md#credentialscontrollerdeletecustomergkcpsz) | **DELETE** /facebook/credentials/{customerId} | 
*FacebookApi* | [**credentialsControllerFindAllUrmvrv**](docs/FacebookApi.md#credentialscontrollerfindallurmvrv) | **GET** /facebook/credentials | 
*FacebookApi* | [**credentialsControllerIsConnectedTfvw6f**](docs/FacebookApi.md#credentialscontrollerisconnectedtfvw6f) | **GET** /facebook/credentials/isConnected | 
*FacebookApi* | [**rawControllerRawRequest1fu5v3Put**](docs/FacebookApi.md#rawcontrollerrawrequest1fu5v3put) | **PUT** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawControllerRawRequest2tg1shGet**](docs/FacebookApi.md#rawcontrollerrawrequest2tg1shget) | **GET** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawControllerRawRequestF1g1cgPost**](docs/FacebookApi.md#rawcontrollerrawrequestf1g1cgpost) | **POST** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawControllerRawRequestG9ig2bPatch**](docs/FacebookApi.md#rawcontrollerrawrequestg9ig2bpatch) | **PATCH** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawControllerRawRequestHkcfxtDelete**](docs/FacebookApi.md#rawcontrollerrawrequesthkcfxtdelete) | **DELETE** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawControllerRawRequestU28fawOptions**](docs/FacebookApi.md#rawcontrollerrawrequestu28fawoptions) | **OPTIONS** /facebook/{customerId}/raw/{externalPath} | 
*FacebookApi* | [**rawControllerRawRequestUdhoymHead**](docs/FacebookApi.md#rawcontrollerrawrequestudhoymhead) | **HEAD** /facebook/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**adAccountsControllerFindAllMln5nd**](docs/GoogleAdsApi.md#adaccountscontrollerfindallmln5nd) | **GET** /googleads/adaccounts | 
*GoogleAdsApi* | [**adAccountsControllerSyncCustomer2j6xn9**](docs/GoogleAdsApi.md#adaccountscontrollersynccustomer2j6xn9) | **PUT** /googleads/{customerId}/adaccounts | 
*GoogleAdsApi* | [**adsControllerCreate5j1f9u**](docs/GoogleAdsApi.md#adscontrollercreate5j1f9u) | **POST** /googleads/ads | 
*GoogleAdsApi* | [**adsControllerFindAllErdkms**](docs/GoogleAdsApi.md#adscontrollerfindallerdkms) | **GET** /googleads/ads | 
*GoogleAdsApi* | [**adsControllerFindOneNutbxl**](docs/GoogleAdsApi.md#adscontrollerfindonenutbxl) | **GET** /googleads/ads/{id} | 
*GoogleAdsApi* | [**adsControllerRemoveAhonpn**](docs/GoogleAdsApi.md#adscontrollerremoveahonpn) | **DELETE** /googleads/ads/{id} | 
*GoogleAdsApi* | [**adsControllerUpdateT99o7f**](docs/GoogleAdsApi.md#adscontrollerupdatet99o7f) | **PATCH** /googleads/ads/{id} | 
*GoogleAdsApi* | [**adsetsControllerCreateX8svw5**](docs/GoogleAdsApi.md#adsetscontrollercreatex8svw5) | **POST** /googleads/adsets | 
*GoogleAdsApi* | [**adsetsControllerFindAll9d7h31**](docs/GoogleAdsApi.md#adsetscontrollerfindall9d7h31) | **GET** /googleads/adsets | 
*GoogleAdsApi* | [**adsetsControllerFindOne3q406b**](docs/GoogleAdsApi.md#adsetscontrollerfindone3q406b) | **GET** /googleads/adsets/{id} | 
*GoogleAdsApi* | [**adsetsControllerRemoveIariyn**](docs/GoogleAdsApi.md#adsetscontrollerremoveiariyn) | **DELETE** /googleads/adsets/{id} | 
*GoogleAdsApi* | [**adsetsControllerUpdateQb6632**](docs/GoogleAdsApi.md#adsetscontrollerupdateqb6632) | **PATCH** /googleads/adsets/{id} | 
*GoogleAdsApi* | [**authControllerGetAccessToken69qgkv**](docs/GoogleAdsApi.md#authcontrollergetaccesstoken69qgkv) | **POST** /googleads/auth | 
*GoogleAdsApi* | [**campaignsControllerCreateWi0t68**](docs/GoogleAdsApi.md#campaignscontrollercreatewi0t68) | **POST** /googleads/campaigns | 
*GoogleAdsApi* | [**campaignsControllerFindAllJazafv**](docs/GoogleAdsApi.md#campaignscontrollerfindalljazafv) | **GET** /googleads/campaigns | 
*GoogleAdsApi* | [**campaignsControllerFindOneU27hua**](docs/GoogleAdsApi.md#campaignscontrollerfindoneu27hua) | **GET** /googleads/campaigns/{id} | 
*GoogleAdsApi* | [**campaignsControllerRemoveWvf99p**](docs/GoogleAdsApi.md#campaignscontrollerremovewvf99p) | **DELETE** /googleads/campaigns/{id} | 
*GoogleAdsApi* | [**campaignsControllerUpdate40ll7r**](docs/GoogleAdsApi.md#campaignscontrollerupdate40ll7r) | **PATCH** /googleads/campaigns/{id} | 
*GoogleAdsApi* | [**credentialsControllerCreateCustomer8qpv6w**](docs/GoogleAdsApi.md#credentialscontrollercreatecustomer8qpv6w) | **POST** /googleads/credentials/customer | 
*GoogleAdsApi* | [**credentialsControllerDeleteCustomerCredentialsSiel2b**](docs/GoogleAdsApi.md#credentialscontrollerdeletecustomercredentialssiel2b) | **DELETE** /googleads/{customerId}/credentials | 
*GoogleAdsApi* | [**credentialsControllerFindAll9quhk2**](docs/GoogleAdsApi.md#credentialscontrollerfindall9quhk2) | **GET** /googleads/credentials | 
*GoogleAdsApi* | [**rawControllerRawRequest60eqvdPost**](docs/GoogleAdsApi.md#rawcontrollerrawrequest60eqvdpost) | **POST** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawControllerRawRequest7vtbrnGet**](docs/GoogleAdsApi.md#rawcontrollerrawrequest7vtbrnget) | **GET** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawControllerRawRequestAfsh4hDelete**](docs/GoogleAdsApi.md#rawcontrollerrawrequestafsh4hdelete) | **DELETE** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawControllerRawRequestD0r8raHead**](docs/GoogleAdsApi.md#rawcontrollerrawrequestd0r8rahead) | **HEAD** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawControllerRawRequestF0ip1pOptions**](docs/GoogleAdsApi.md#rawcontrollerrawrequestf0ip1poptions) | **OPTIONS** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawControllerRawRequestH2cub1Put**](docs/GoogleAdsApi.md#rawcontrollerrawrequesth2cub1put) | **PUT** /googleads/{customerId}/raw/{externalPath} | 
*GoogleAdsApi* | [**rawControllerRawRequestWg2qdkPatch**](docs/GoogleAdsApi.md#rawcontrollerrawrequestwg2qdkpatch) | **PATCH** /googleads/{customerId}/raw/{externalPath} | 
*PinterestApi* | [**convertAuthCode**](docs/PinterestApi.md#convertauthcode) | **POST** /pinterest/auth | Convert Pinterest auth code
*PinterestApi* | [**deletePinterestCustomerCredentials**](docs/PinterestApi.md#deletepinterestcustomercredentials) | **DELETE** /pinterest/credentials/{customerId} | Delete Pinterest credentials for a customer
*PinterestApi* | [**rawRequest**](docs/PinterestApi.md#rawrequest) | **GET** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequest_0**](docs/PinterestApi.md#rawrequest_0) | **HEAD** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequest_1**](docs/PinterestApi.md#rawrequest_1) | **PUT** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequest_2**](docs/PinterestApi.md#rawrequest_2) | **POST** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequest_3**](docs/PinterestApi.md#rawrequest_3) | **DELETE** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequest_4**](docs/PinterestApi.md#rawrequest_4) | **PATCH** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**rawRequest_5**](docs/PinterestApi.md#rawrequest_5) | **OPTIONS** /pinterest/{customerId}/raw/{externalPath} | Proxy raw requests to the Pinterest API
*PinterestApi* | [**storePinterestCustomerCredentials**](docs/PinterestApi.md#storepinterestcustomercredentials) | **POST** /pinterest/credentials/customer | Store Pinterest credentials for a customer
*ReportingApi* | [**reportingControllerGetReportIxk9wf**](docs/ReportingApi.md#reportingcontrollergetreportixk9wf) | **GET** /reporting | 
*TheTradeDeskApi* | [**rawRequest**](docs/TheTradeDeskApi.md#rawrequest) | **GET** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequest_0**](docs/TheTradeDeskApi.md#rawrequest_0) | **HEAD** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequest_1**](docs/TheTradeDeskApi.md#rawrequest_1) | **PUT** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequest_2**](docs/TheTradeDeskApi.md#rawrequest_2) | **POST** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequest_3**](docs/TheTradeDeskApi.md#rawrequest_3) | **DELETE** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequest_4**](docs/TheTradeDeskApi.md#rawrequest_4) | **PATCH** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**rawRequest_5**](docs/TheTradeDeskApi.md#rawrequest_5) | **OPTIONS** /thetradedesk/{customerId}/raw/{externalPath} | Proxy raw requests to the The Trade Desk API
*TheTradeDeskApi* | [**storeCustomerCredentials**](docs/TheTradeDeskApi.md#storecustomercredentials) | **POST** /thetradedesk/credentials/customer | Login to The Trade Desk


### Documentation For Models

 - [ActiveAgentCreateCredentialDto](docs/ActiveAgentCreateCredentialDto.md)
 - [ActiveAgentOrderDto](docs/ActiveAgentOrderDto.md)
 - [Ad](docs/Ad.md)
 - [AdSet](docs/AdSet.md)
 - [Campaign](docs/Campaign.md)
 - [CreateAdSetDto](docs/CreateAdSetDto.md)
 - [CreateAdSetDtoSettingsInner](docs/CreateAdSetDtoSettingsInner.md)
 - [CreateAdSetDtoTargetingsInner](docs/CreateAdSetDtoTargetingsInner.md)
 - [CreateCustomerDto](docs/CreateCustomerDto.md)
 - [CreateFacebookAuthDto](docs/CreateFacebookAuthDto.md)
 - [CreateGoogleAdsAuthDto](docs/CreateGoogleAdsAuthDto.md)
 - [CreatePinterestAuthDto](docs/CreatePinterestAuthDto.md)
 - [CreateSettingDto](docs/CreateSettingDto.md)
 - [CreateSettingDtoSettingsInner](docs/CreateSettingDtoSettingsInner.md)
 - [CreateTargetingDto](docs/CreateTargetingDto.md)
 - [CreateTargetingDtoTargetingsInner](docs/CreateTargetingDtoTargetingsInner.md)
 - [DailyBudgetDto](docs/DailyBudgetDto.md)
 - [FacebookAdAccountWrapper](docs/FacebookAdAccountWrapper.md)
 - [FacebookCreateCredentialDto](docs/FacebookCreateCredentialDto.md)
 - [FrequencyCappingDto](docs/FrequencyCappingDto.md)
 - [GoogleAdsAdAccountWrapper](docs/GoogleAdsAdAccountWrapper.md)
 - [GoogleAdsCreateCredentialDto](docs/GoogleAdsCreateCredentialDto.md)
 - [LoginDto](docs/LoginDto.md)
 - [MaximumCPMDto](docs/MaximumCPMDto.md)
 - [MaximumDailyImpressionsDto](docs/MaximumDailyImpressionsDto.md)
 - [PacingDto](docs/PacingDto.md)
 - [PinterestCreateCredentialDto](docs/PinterestCreateCredentialDto.md)
 - [RealtimeBiddingStrategyDto](docs/RealtimeBiddingStrategyDto.md)
 - [RedirectUriDTO](docs/RedirectUriDTO.md)
 - [RuntimeBudget](docs/RuntimeBudget.md)
 - [SessionTokenDto](docs/SessionTokenDto.md)
 - [SessionTokenVerifyDto](docs/SessionTokenVerifyDto.md)
 - [TheTradeDeskCreateCredentialsDto](docs/TheTradeDeskCreateCredentialsDto.md)
 - [UrlTargetingDto](docs/UrlTargetingDto.md)
 - [ZipcodeDto](docs/ZipcodeDto.md)
 - [ZipcodeGeoTargetingDto](docs/ZipcodeGeoTargetingDto.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="bearerAuth"></a>
### bearerAuth

- **Type**: Bearer authentication (JWT)

