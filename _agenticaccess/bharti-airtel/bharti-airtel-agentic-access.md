---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 33
api_specs:
- filename: bharti-airtel-iq-sms-openapi.yml
  format: yaml
  label: Airtel IQ SMS API
  slug: airtel-iq-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iq-sms-openapi.yml
- filename: bharti-airtel-iq-reporting-openapi.yml
  format: yaml
  label: Airtel IQ Reporting API
  slug: airtel-iq-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iq-reporting-openapi.yml
- filename: bharti-airtel-iot-openapi.yml
  format: yaml
  label: Airtel IoT API
  slug: airtel-iot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-iot-openapi.yml
- filename: bharti-airtel-locate-openapi.yml
  format: yaml
  label: Airtel Locate API
  slug: airtel-locate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/openapi/bharti-airtel-locate-openapi.yml
consequence_counts:
  physical: 8
  read: 33
  write: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bharti Airtel Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send-sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send-sms-bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send-sms-cm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/send-sms-csv
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulk/sim/download/template
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/custom/message
operation_count: 68
overview: 'Bharti Airtel exposes 68 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read, 27 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bharti Airtel
provider_slug: bharti-airtel
slug: bharti-airtel-agentic-access
source_filename: bharti-airtel-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/bharti-airtel-iot-openapi.yml, openapi/bharti-airtel-iq-reporting-openapi.yml,\n  openapi/bharti-airtel-iq-sms-openapi.yml, openapi/bharti-airtel-locate-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    acting: 35\n    connected: 33\n  by_consequence:\n    write: 27\n    physical: 8\n    read: 33\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/v2/generate/authtoken\n  method: post\n  operationId: generateAccessTokenUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /auth/v2/refresh/authtoken\n  method: post\n  operationId: refreshAccessTokenUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/activate/test/sims\n  method: post\n  operationId: activateTestSimsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/activate/sim/from/test\n  method: post\n  operationId: activateSimFromTestUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/change/plan\n  method: post\n  operationId: changePlanUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk/sim/download/template\n  method: post\n  operationId: downloadBulkOrderTemplateUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk/sim/upload\n  method: post\n\
  \  operationId: bulkUploadUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk/download/history\n  method: get\n  operationId: fetchDownloadHistoryUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/download/{downloadFileId}\n  method: get\n  operationId: downloadTemplateFileUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/all\n  method: get\n  operationId: fetchJobsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /job/{jobId}/order\n  method: get\n  operationId: fetchOrdersUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sim/device/info\n  method: get\n  operationId: fetchDeviceInfoUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sim/data/usage\n  method: get\n  operationId: fetchDataUsageUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wt/numbers\n  method: get\n  operationId: fetchSMSWhitelistedNumbersUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wt/numbers/batch\n  method: post\n  operationId: smsWhitelistedNumbersBatchUsingPOST\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kyc/sim/details\n  method: get\n  operationId: fetchSimKycDetailsListUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kyc/sim/update\n  method: post\n  operationId: updateSimKycDetailsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/quota\n  method: get\n  operationId: fetchSMSQuotaDetailsUsingGET\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/history\n  method: get\n  operationId: fetchPurchaseHistoryUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /template/\n  method: get\n  operationId: fetchTemplatesUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /send\n  method: post\n  operationId: sendSMSUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/custom/message\n  method: post\n  operationId:\
  \ sendCustomSMSUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /download/batch/template\n  method: post\n  operationId: downloadBulkSMSTemplateUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/batch\n  method: post\n  operationId: sendBatchSMSUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /box\n  method: get\n  operationId: fetchMessageHistoryUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/history\n  method: get\n  operationId: fetchJobHistoryUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/detail\n  method: get\n  operationId: fetchSmsOrderDetailsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /device/diagnose/radius\n  method: get\n  operationId: deviceDiagnoseRadiusUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /details/\n  method: get\n  operationId: fetchCustomerProfileUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /details/stats\n  method: get\n  operationId: fetchCustomerStatsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /details/plans\n  method: get\n  operationId: fetchCustomerPlansUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/sim/activate\n  method: post\n  operationId: activateSimsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/sim/swap\n  method: post\n  operationId: swapSimUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk/dataUsages/download\n  method: post\n  operationId: downloadDataUsagesUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice/numbers\n  method: get\n  operationId: fetchVoiceWhitelistedNumbersUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /voice/numbers\n  method: post\n  operationId: updateVoiceWhitelistNumberUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk/sim/inventory/download\n  method: get\n  operationId: downloadSimInventoryOrderUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /details/baskets\n  method: get\n  operationId: fetchCustomerBasketsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/sim/voluntary/suspend\n  method: post\n  operationId: safeCustodyUsingPOST\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/sim/voluntary/resume\n  method: post\n  operationId: outOfSafeCustodyUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/temp/disconnect\n  method: post\n  operationId: tempDisconnectionUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /job/td/resume\n  method: post\n  operationId: tdResumeUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /details/basket/{basketId}/sims\n  method: get\n  operationId: fetchCustomerSimsUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sampleCdr\n  method: post\n  operationId: postSampleCdrUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/send-sms\n  method: get\n  operationId: sendSmsUsingGET\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/send-sms\n  method: post\n  operationId: sendSmsUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/send-sms-bulk\n  method: post\n  operationId: sendSmsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/send-sms-cm\n  method:\
  \ post\n  operationId: sendSmsViaCsvUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/send-sms-csv\n  method: post\n  operationId: sendSmsViaCsvUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/oauth2_token\n  method: post\n  operationId: getOrCreateOauthTokenUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/resources\n  method: get\n  operationId: findAllUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/resources/consent\n  method: post\n  operationId: initiateConsentUsingPOST_3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/resources/{msisdn}\n  method: get\n  operationId: searchUsingGET_2\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/resources/{msisdn}\n  method: delete\n  operationId: deleteResourceUsingDELETE_3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/resources/{msisdn}\n  method: patch\n  operationId: patchResourceUsingPATCH_3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/resources/{msisdn}/consent\n  method:\
  \ get\n  operationId: getConsentUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/resources/{msisdn}/location\n  method: get\n  operationId: getLocationUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/resources/{msisdn}/validation/address\n  method: post\n  operationId: addressValidationUsingPOST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/tenants\n  method: get\n  operationId: getCustomerTenantsUsingGET_1\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/tenants/consent/purpose\n  method: get\n  operationId: getAllConsentPurposeUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources\n  method: get\n  operationId: findAllUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources/consent\n  method: post\n  operationId: initiateConsentUsingPOST_4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources/{msisdn}\n  method: get\n  operationId: searchUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources/{msisdn}\n  method: delete\n  operationId: deleteResourceUsingDELETE_4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources/{msisdn}\n  method: patch\n  operationId: patchResourceUsingPATCH_4\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources/{msisdn}/consent\n  method: get\n  operationId: getConsentUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources/{msisdn}/location\n  method: get\n  operationId: getLocationForTenantsUsingGET_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate/apis/customers/{customerBaId}/tenants/{tenantId}/resources/{msisdn}/validation/address\n  method: post\n  operationId: addressValidationForTenantsUsingPOST_1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bharti-airtel/refs/heads/main/agentic-access/bharti-airtel-agentic-access.yml
summary_line: 68 operations · 35 acting
tags:
- Telecommunications
- India
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- CPaaS
- Messaging
- SMS
- RCS
- Voice
- IoT
- M2M
- Device Location
- Broadband
- 5G
- Identity Verification
- Carrier Billing
- Consent Management
---
