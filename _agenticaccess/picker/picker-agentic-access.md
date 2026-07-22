---
acting_count: 254
action_class_counts:
  acting: 254
  connected: 159
api_specs:
- filename: picker-openapi-original.json
  format: json
  label: Picker API
  slug: picker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/picker/refs/heads/main/openapi/picker-openapi-original.json
consequence_counts:
  physical: 51
  read: 159
  safety-critical: 2
  write: 201
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Picker Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /user/resetPassword
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /user/verifyForgotPasswordOTP
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounting/generateBusinessPayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounting/generateBusinessPaymentBulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /accounting/generateWeeklyDriverPayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /accounting/refundBalanceTransactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /admin/changeDriverPaymentType
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/makeChargesToBooking
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/makeRefund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/sendEmailTo
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/sendInvoiceEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/sendPushToUsers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/sendWeeklyPaymentEmail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/sendWeeklyPaymentMail
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/totalOrderRequests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /admin/updateAllDriversPaymentBalance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/addCard
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pushShopifyOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pushSpoonityOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/pushVtexOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/sendChatbotBookingRate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /billing/sendBillToDatil
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/sendBillsToDatil
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /booking/addProofOfDelivery
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /booking/assignBookingManually
operation_count: 413
overview: 'Picker exposes 413 API operations that an AI agent could call, of which 254 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 159 read, 201 write, 51 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Picker
provider_slug: picker
slug: picker-agentic-access
source_filename: picker-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/picker-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 413\n  by_action_class:\n    connected: 159\n    acting: 254\n  by_consequence:\n    read: 159\n    write: 201\n    physical: 51\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /cancel\n  method: get\n  operationId: getCancel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getContactUsDetails\n  method: get\n  operationId: getGetcontactusdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /health-check\n  method: get\n  operationId: getHealthcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mass-delivery\n  method: get\n  operationId: getMassdelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /share-my-ride\n  method: get\n  operationId: getSharemyride\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /share-my-ride\n  method: post\n  operationId: postSharemyride\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /{param*}\n  method: get\n  operationId: getParam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getAPICharges\n  method: get\n  operationId: getAccountingGetapicharges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getAllBusinessesBalanceTransactionDetails\n  method: get\n  operationId: getAccountingGetallbusinessesbalancetransactiondetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getAllBusinessesTransactions\n  method: get\n  operationId: getAccountingGetallbusinessestransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /accounting/getAllBusinessesTransactionsSummary\n  method: get\n  operationId: getAccountingGetallbusinessestransactionssummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getAllDriversBonusTransactions\n  method: get\n  operationId: getAccountingGetalldriversbonustransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getAllDriversDeliveryTransactions\n  method: get\n  operationId: getAccountingGetalldriversdeliverytransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getAllDriversDeliveryTransactionsSummary\n  method: get\n  operationId: getAccountingGetalldriversdeliverytransactionssummary\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getCompanyTransactions\n  method: get\n  operationId: getAccountingGetcompanytransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getDriverDeliveryTransactionsDetails\n  method: get\n  operationId: getAccountingGetdriverdeliverytransactionsdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounting/getPickerBonusTransactionsDetails\n  method: get\n  operationId: getAccountingGetpickerbonustransactionsdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/addBusinessAccessToUser\n\
  \  method: get\n  operationId: getAdminAddbusinessaccesstouser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/assignReasons\n  method: get\n  operationId: getAdminAssignreasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/bookings\n  method: get\n  operationId: getAdminBookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/cancelBookingReasons\n  method: get\n  operationId: getAdminCancelbookingreasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/deleteBusinessAccessToUser\n  method: get\n  operationId: getAdminDeletebusinessaccesstouser\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/driversWorkBalance\n  method: get\n  operationId: getAdminDriversworkbalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllAvailabeBooking\n  method: get\n  operationId: getAdminGetallavailabebooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllBusinesses\n  method: get\n  operationId: getAdminGetallbusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllBusinessesTransactions\n  method: get\n  operationId: getAdminGetallbusinessestransactions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllCancelReasons\n  method: get\n  operationId: getAdminGetallcancelreasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllDriverTags\n  method: get\n  operationId: getAdminGetalldrivertags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllPickersBalanceTransactions\n  method: get\n  operationId: getAdminGetallpickersbalancetransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllPickersOrderTransactions\n  method: get\n  operationId: getAdminGetallpickersordertransactions\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getAllUsers\n  method: get\n  operationId: getAdminGetallusers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getBanners\n  method: get\n  operationId: getAdminGetbanners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getBookingDetails\n  method: get\n  operationId: getAdminGetbookingdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getBookingInfo\n  method: get\n  operationId: getAdminGetbookinginfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /admin/getBookingTransactions\n  method: get\n  operationId: getAdminGetbookingtransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getBookingsStats\n  method: get\n  operationId: getAdminGetbookingsstats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getBusinessBalanceTransactionDetails\n  method: get\n  operationId: getAdminGetbusinessbalancetransactiondetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getBusinessByName\n  method: get\n  operationId: getAdminGetbusinessbyname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n    \
  \  max-ttl: 3600\n    audit: none\n- path: /admin/getBusinessInfo\n  method: get\n  operationId: getAdminGetbusinessinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getBusinessesByIds\n  method: get\n  operationId: getAdminGetbusinessesbyids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getCSVDataForAdmin\n  method: get\n  operationId: getAdminGetcsvdataforadmin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getDashboardCount\n  method: get\n  operationId: getAdminGetdashboardcount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getDriverBanners\n\
  \  method: get\n  operationId: getAdminGetdriverbanners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getOngoingBooking\n  method: get\n  operationId: getAdminGetongoingbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getPastBooking\n  method: get\n  operationId: getAdminGetpastbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getPickerBalanceTransactionsDetails\n  method: get\n  operationId: getAdminGetpickerbalancetransactionsdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getPickerDetails\n  method: get\n  operationId:\
  \ getAdminGetpickerdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getPickerOrderTransactionDetails\n  method: get\n  operationId: getAdminGetpickerordertransactiondetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getPickerPay\n  method: get\n  operationId: getAdminGetpickerpay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getQueryByCustomer\n  method: get\n  operationId: getAdminGetquerybycustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getServiceProviderInfo\n  method: get\n  operationId: getAdminGetserviceproviderinfo\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getTransactionFraudInformation\n  method: get\n  operationId: getAdminGettransactionfraudinformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getTransactionsByCode\n  method: get\n  operationId: getAdminGettransactionsbycode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getUserCardInfo\n  method: get\n  operationId: getAdminGetusercardinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/getUserHistory\n  method: get\n  operationId: getAdminGetuserhistory\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/listDefaultSettings\n  method: get\n  operationId: getAdminListdefaultsettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/searchAuthorizationCode\n  method: get\n  operationId: getAdminSearchauthorizationcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/userBookings\n  method: get\n  operationId: getAdminUserbookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/userDetails\n  method: get\n  operationId: getAdminUserdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/warningBookings\n  method: get\n  operationId: getAdminWarningbookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /angular4-docs/{param*}\n  method: get\n  operationId: getAngular4docsParam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/getBookingDetails\n  method: get\n  operationId: getApiGetbookingdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/getChatbotBooking\n  method: get\n  operationId: getApiGetchatbotbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/getDriver\n\
  \  method: get\n  operationId: getApiGetdriver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/getDriverById\n  method: get\n  operationId: getApiGetdriverbyid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/getDrivers\n  method: get\n  operationId: getApiGetdrivers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/getPastBooking\n  method: get\n  operationId: getApiGetpastbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks\n  method: get\n  operationId: getApiWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/webhooks\n  method: post\n  operationId: postApiWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/webhooks\n  method: delete\n  operationId: deleteApiWebhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /appVersion/getCurrentVersions\n  method: get\n  operationId: getAppversionGetcurrentversions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /billing/driversBills\n  method: get\n  operationId: getBillingDriversbills\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/getAllUsersName\n  method: get\n  operationId: getBillingGetallusersname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/getBillDetails\n  method: get\n  operationId: getBillingGetbilldetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getAllAvailabeBooking\n  method: get\n  operationId: getBookingGetallavailabebooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getAllBids\n\
  \  method: get\n  operationId: getBookingGetallbids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getAllBookingDetails\n  method: get\n  operationId: getBookingGetallbookingdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getAmountlogs\n  method: get\n  operationId: getBookingGetamountlogs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getBookingDetails\n  method: get\n  operationId: getBookingGetbookingdetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getBookingReport\n  method: get\n  operationId: getBookingGetbookingreport\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getBookingRoute\n  method: get\n  operationId: getBookingGetbookingroute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getOngoingBooking\n  method: get\n  operationId: getBookingGetongoingbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getPastBooking\n  method: get\n  operationId: getBookingGetpastbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/getProductList\n  method: get\n  operationId: getBookingGetproductlist\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/preCheckout\n  method: get\n  operationId: getBookingPrecheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /booking/preCheckout\n  method: post\n  operationId: postBookingPrecheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bookingAssignment/listBookingFloatSetting\n  method: get\n  operationId: getBookingassignmentListbookingfloatsetting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /bookingIssues/getBookingIssues\n  method: get\n  operationId: getBookingissuesGetbookingissues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/getAllBookingsDashBoard\n  method: get\n  operationId: getBookingsGetallbookingsdashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/getCoportatesAllBookings\n  method: get\n  operationId: getBookingsGetcoportatesallbookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bookings/getCorporateBookingsByUserId\n  method: get\n  operationId: getBookingsGetcorporatebookingsbyuserid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /business/categories\n  method: get\n  operationId: getBusinessCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/categoriesByUserId\n  method: get\n  operationId: getBusinessCategoriesbyuserid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/checkAvailableNames\n  method: get\n  operationId: getBusinessCheckavailablenames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getAccountInfoIntegrationDashboard\n  method: get\n  operationId: getBusinessGetaccountinfointegrationdashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getAssociatedBusiness\n  method: get\n  operationId: getBusinessGetassociatedbusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBookings\n  method: get\n  operationId: getBusinessGetbookings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBookingsDataByDatesDashboard\n  method: get\n  operationId: getBusinessGetbookingsdatabydatesdashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBookingsIntegrationDashboard\n  method: get\n  operationId: getBusinessGetbookingsintegrationdashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBusinessCategories\n  method: get\n  operationId: getBusinessGetbusinesscategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBusinessInfo\n  method: get\n  operationId: getBusinessGetbusinessinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBusinessInfoAfterLanding\n  method: get\n  operationId: getBusinessGetbusinessinfoafterlanding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBusinessInfoByUserId\n  method: get\n  operationId: getBusinessGetbusinessinfobyuserid\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBusinessesByDistance\n  method: get\n  operationId: getBusinessGetbusinessesbydistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBusinessesBySubcategory\n  method: get\n  operationId: getBusinessGetbusinessesbysubcategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getBusinessesGeneralInfo\n  method: get\n  operationId: getBusinessGetbusinessesgeneralinfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/getStats\n  method: get\n  operationId: getBusinessGetstats\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/landing\n  method: get\n  operationId: getBusinessLanding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/products\n  method: get\n  operationId: getBusinessProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/reports\n  method: get\n  operationId: getBusinessReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business/sendSundayReports\n  method: get\n  operationId: getBusinessSendsundayreports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /business/turnOffOnBusinessById\n  method: get\n  operationId: getBusinessTurnoffonbusinessbyid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/getChatForBooking\n  method: get\n  operationId: getChatGetchatforbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chat/getChatForBookingByComeChat\n  method: get\n  operationId: getChatGetchatforbookingbycomechat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/getMessage\n  method: get\n  operationId: getClientGetmessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/availableServiceProvider\n\
  \  method: get\n  operationId: getCustomerAvailableserviceprovider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/bookingAddresses\n  method: get\n  operationId: getCustomerBookingaddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/bookingPaymentHistory\n  method: get\n  operationId: getCustomerBookingpaymenthistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/bookingPaymentPending\n  method: get\n  operationId: getCustomerBookingpaymentpending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/getFavorites\n  method: get\n\
  \  operationId: getCustomerGetfavorites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/getPastBooking\n  method: get\n  operationId: getCustomerGetpastbooking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/listServiceLocation\n  method: get\n  operationId: getCustomerListservicelocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/search\n  method: get\n  operationId: getCustomerSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/totalPayments\n  method: get\n  operationId: getCustomerTotalpayments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/getAllAvailableDriver\n  method: get\n  operationId: getDriverGetallavailabledriver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/getAllAvailableDriverMyFleet\n  method: get\n  operationId: getDriverGetallavailabledrivermyfleet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/getAllDriver\n  method: get\n  operationId: getDriverGetalldriver\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/getDriverBalances\n  method: get\n  operationId: getDriverGetdriverbalances\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/getDriverTracking\n  method: get\n  operationId: getDriverGetdrivertracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/getEarnings\n  method: get\n  operationId: getDriverGetearnings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/getVehicleDetails\n  method: get\n  operationId: getDriverGetvehicledetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /driver/listVehicleTypeAndCompany\n  method: get\n  operationId: getDriverListvehicletypeandcompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /notification/getAllNotification\n  method: get\n  operationId: getNotificationGetallnotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /promo/getAllUserPromo\n  method: get\n  operationId: getPromoGetalluserpromo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /promo/listAllPromo\n  method: get\n  operationId: getPromoListallpromo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /promo/promoDetails\n  method: get\n  operationId: getPromoPromodetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/reports\n\
  \  method: get\n  operationId: getPublicReports\n  x-agentic-access:\n   \n\n# --- truncated at 32 KB (127 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/picker/refs/heads/main/agentic-access/picker-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picker/refs/heads/main/agentic-access/picker-agentic-access.yml
summary_line: 413 operations · 254 acting · 2 human-in-the-loop
tags:
- Company
- Logistics
- Delivery
- Last Mile
- Courier
- E-commerce
- Shipping
- Tracking
- Latin America
- Fleet Management
---
