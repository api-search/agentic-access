---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 35
api_specs:
- filename: con-edison-applicationinformation-api-openapi.yml
  format: yaml
  label: Con Edison Application Information API
  slug: con-edison-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-applicationinformation-api-openapi.yml
- filename: con-edison-authorization-api-openapi.yml
  format: yaml
  label: Con Edison Authorization API
  slug: con-edison-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-authorization-api-openapi.yml
- filename: con-edison-batch-api-openapi.yml
  format: yaml
  label: Con Edison Batch API
  slug: con-edison-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-batch-api-openapi.yml
- filename: con-edison-electricpowerusagesummary-api-openapi.yml
  format: yaml
  label: Con Edison Electric Power Usage Summary API
  slug: con-edison-electricpowerusagesummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-electricpowerusagesummary-api-openapi.yml
- filename: con-edison-intervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Interval Block API
  slug: con-edison-intervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-intervalblock-api-openapi.yml
- filename: con-edison-localtimeparameters-api-openapi.yml
  format: yaml
  label: Con Edison Local Time Parameters API
  slug: con-edison-localtimeparameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-localtimeparameters-api-openapi.yml
- filename: con-edison-meterreading-api-openapi.yml
  format: yaml
  label: Con Edison Meter Reading API
  slug: con-edison-meterreading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-meterreading-api-openapi.yml
- filename: con-edison-readingtype-api-openapi.yml
  format: yaml
  label: Con Edison Reading Type API
  slug: con-edison-readingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-readingtype-api-openapi.yml
- filename: con-edison-realtimebatch-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Batch API
  slug: con-edison-realtimebatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimebatch-api-openapi.yml
- filename: con-edison-realtimeintervalblock-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Interval Block API
  slug: con-edison-realtimeintervalblock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimeintervalblock-api-openapi.yml
- filename: con-edison-realtimereadingtype-api-openapi.yml
  format: yaml
  label: Con Edison Real Time Reading Type API
  slug: con-edison-realtimereadingtype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-realtimereadingtype-api-openapi.yml
- filename: con-edison-retailcustomer-api-openapi.yml
  format: yaml
  label: Con Edison Retail Customer API
  slug: con-edison-retailcustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-retailcustomer-api-openapi.yml
- filename: con-edison-servicestatus-api-openapi.yml
  format: yaml
  label: Con Edison Service Status API
  slug: con-edison-servicestatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-servicestatus-api-openapi.yml
- filename: con-edison-usagepoint-api-openapi.yml
  format: yaml
  label: Con Edison Usage Point API
  slug: con-edison-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/openapi/con-edison-usagepoint-api-openapi.yml
consequence_counts:
  read: 35
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Con Edison Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'Con Edison exposes 37 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 35 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Con Edison
provider_slug: con-edison
slug: con-edison-agentic-access
source_filename: con-edison-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/con-edison-green-button-connect-my-data-swagger.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 35\n    acting: 2\n  by_consequence:\n    read: 35\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /resource/ApplicationInformation/{applicationInformationId}\n  method: get\n  operationId: getThirdPartyApplicationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Authorization\n  method: get\n  operationId: Get all Third Party Authorizations\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Authorization/{authorizationId}\n  method: get\n  operationId: Get Third Party Authorization by ID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/ReadServiceStatus\n  method: get\n  operationId: readServiceStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/Token\n  method: post\n  operationId: Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource/Batch/Bulk/{bulkId}\n  method: get\n  operationId: getAllUsageDataInBatch\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Batch/Subscription/{subscriptionId}\n  method: get\n  operationId: getAllUsageDataForSubscriptionInBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Batch/Subscription/{subscriptionId}/UsagePoint/{usagePointId}\n  method: get\n  operationId: getUsagePointBySubscriptionInBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Batch/RetailCustomer/{subscriptionId}\n  method: get\n  operationId: getCustomerInformationInBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/MeterReading/{meterReadingId}/IntervalBlock\n\
  \  method: get\n  operationId: getAllIntervalBlocksForUsagePointMeterReadingInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/MeterReading/{meterReadingId}/IntervalBlock/{intervalBlockId}\n  method: get\n  operationId: getIntervalBlocksForUsagePointMeterReadingInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/LocalTimeParameters\n  method: get\n  operationId: getLocalTimeParameters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/LocalTimeParameters/{localTimeParameterId}\n  method: get\n  operationId: getLocalTimeParametersById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/MeterReading\n  method: get\n  operationId: getAllMeterReadingsForUsagePointInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/MeterReading/{meterReadingId}\n  method: get\n  operationId: getMeterReadingForUsagePointInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/ReadingType\n  method: get\n  operationId: getAllReadingTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/ReadingType/{readingTypeId}\n\
  \  method: get\n  operationId: getReadingTypesById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/RealTime/Batch/Bulk/{bulkId}\n  method: get\n  operationId: getAllRealTimeUsageDataInBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/RealTime/Batch/Subscription/{subscriptionId}\n  method: get\n  operationId: getAllRealTimeUsageDataForSubscriptionInBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/RealTime/Batch/Subscription/{subscriptionId}/UsagePoint/{usagePointId}\n  method: get\n  operationId: getRealTimeUsagePointBySubscriptionInBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/RealTime/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/MeterReading/{meterReadingId}/IntervalBlock\n  method: get\n  operationId: getAllRealTimeIntervalBlocksForUsagePointMeterReadingInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/RealTime/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/MeterReading/{meterReadingId}/IntervalBlock/{intervalBlockId}\n  method: get\n  operationId: getRealTimeIntervalBlockForUsagePointMeterReadingInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/RealTime/ReadingType\n  method: get\n  operationId: getAllRealTimeReadingTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/RealTime/ReadingType/{readingTypeId}\n  method: get\n  operationId: getRealTimeReadingTypeById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}\n  method: get\n  operationId: getCustomerInformationBySubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount\n  method: get\n  operationId: getCustomerAccountInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount/{accountId}\n  method: get\n  operationId: getCustomerAccountByAccountIdInSubscription\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount/{accountId}/CustomerAgreement\n  method: get\n  operationId: getCustomerAgreementByAccountIdInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount/{accountId}/CustomerAgreement/{customerAgreementId}\n  method: get\n  operationId: getCustomerAgreementByCustomerAgreementId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount/{accountId}/CustomerAgreement/{customerAgreementId}/ServiceLocation\n  method: get\n  operationId: getAllServiceLocationByCustomerAgreementIdAndAccountIdInSubscription\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount/{accountId}/CustomerAgreement/{customerAgreementId}/ServiceLocation/{serviceLocationId}\n  method: get\n  operationId: getServiceLocationByServiceLocationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount/{accountId}/CustomerAgreement/{customerAgreementId}/ServiceLocation/{serviceLocationId}/Meter\n  method: get\n  operationId: getAllMetersForServiceLocationInSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Customer/{subscriptionId}/CustomerAccount/{accountId}/CustomerAgreement/{customerAgreementId}/ServiceLocation/{serviceLocationId}/Meter/{serialNumber}\n\
  \  method: get\n  operationId: getMeterBySerialNumberId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/UsageSummary\n  method: get\n  operationId: getAllElectricPowerUsageSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Subscription/{subscriptionId}/UsagePoint/{usagePointId}/UsageSummary/{usageSummaryId}\n  method: post\n  operationId: getAllElectricPowerUsageSummariesById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resource/Subscription/{subscriptionId}/UsagePoint\n\
  \  method: get\n  operationId: getAllUsagePointsBySubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/Subscription/{subscriptionId}/UsagePoint/{usagePointId}\n  method: get\n  operationId: getUsagePointsForSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/con-edison/refs/heads/main/agentic-access/con-edison-agentic-access.yml
summary_line: 37 operations · 2 acting
tags:
- Energy
- United States
- New York
- Utilities
- Electricity
- Gas
- Steam
- Smart Metering
- Green Button
- Energy Data
- Grid
- Distribution
- Hosting Capacity
- Distributed Energy Resources
- Solar
- EV Charging
- Demand Response
---
