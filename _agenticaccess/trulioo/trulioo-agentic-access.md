---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 34
api_specs:
- filename: trulioo-verifications-api-openapi.yml
  format: yaml
  label: Trulioo Verifications API
  slug: trulioo-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-verifications-api-openapi.yml
- filename: trulioo-configuration-api-openapi.yml
  format: yaml
  label: Trulioo Configuration API
  slug: trulioo-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-configuration-api-openapi.yml
- filename: trulioo-connection-api-openapi.yml
  format: yaml
  label: Trulioo Connection API
  slug: trulioo-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-connection-api-openapi.yml
- filename: trulioo-business-verification-api-openapi.yml
  format: yaml
  label: Trulioo Business Verification API
  slug: trulioo-business-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-verification-api-openapi.yml
- filename: trulioo-person-fraud-api-openapi.yml
  format: yaml
  label: Trulioo Person Fraud API
  slug: trulioo-person-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-person-fraud-api-openapi.yml
- filename: trulioo-document-verification-api-openapi.yml
  format: yaml
  label: Trulioo Identity Document Verification API
  slug: trulioo-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-document-verification-api-openapi.yml
- filename: trulioo-platform-api-openapi.yml
  format: yaml
  label: Trulioo Platform API
  slug: trulioo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-platform-api-openapi.yml
consequence_counts:
  physical: 1
  read: 34
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trulioo Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /customer/v2/events
operation_count: 54
overview: 'Trulioo exposes 54 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 34 read, 19 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Trulioo
provider_slug: trulioo
slug: trulioo-agentic-access
source_filename: trulioo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/trulioo-business-verification-api-openapi.yml, openapi/trulioo-configuration-api-openapi.yml,\n  openapi/trulioo-connection-api-openapi.yml, openapi/trulioo-document-verification-api-openapi.yml,\n  openapi/trulioo-person-fraud-api-openapi.yml, openapi/trulioo-platform-api-openapi.yml, openapi/trulioo-verifications-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 54\n  by_action_class:\n    acting: 20\n    connected: 34\n  by_consequence:\n    write: 19\n    read: 34\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/business/search\n  method: post\n  operationId: businessSearch\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/business/verify\n  method: post\n  operationId: businessVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/business/search/transactionrecord/{transactionRecordId}\n  method: get\n  operationId: getBusinessSearchResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/business/report/{transactionRecordId}\n  method: get\n  operationId: getBusinessReport\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/business/countryJOI\n  method: get\n  operationId: getAllJurisdictionsOfIncorporation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/business/countryJOI/{countryCode}\n  method: get\n  operationId: getJurisdictionsOfIncorporationPerCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/business/businessregistrationnumbers\n  method: get\n  operationId: getAllBusinessRegistrationNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/business/businessregistrationnumbers/{countryCode}\n  method: get\n  operationId: getBusinessRegistrationNumbersByCountry\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/packages\n  method: get\n  operationId: getPackages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/countrycodes/{configurationName}\n  method: get\n  operationId: getCountryCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/countrysubdivisions/{countryCode}\n  method: get\n  operationId: getCountrySubdivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/fields/{configurationName}/{countryCode}\n  method: get\n  operationId: getFields\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/fields/{configurationName}/{countryCode}/recommended\n  method: get\n  operationId: getRecommendedFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/datasources/{configurationName}/{countryCode}\n  method: get\n  operationId: getDatasources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/consents/{configurationName}/{countryCode}\n  method: get\n  operationId: getConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/consents/{configurationName}/{countryCode}/detail\n  method: get\n\
  \  operationId: getDetailedConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/testentities/{configurationName}/{countryCode}\n  method: get\n  operationId: getTestEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/configuration/documentTypes/{countryCode}\n  method: get\n  operationId: getDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/connection/sayhello/{name}\n  method: get\n  operationId: sayHello\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/connection/testauthentication\n  method: get\n  operationId: testAuthentication\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/verifications/documentverification/verify\n  method: post\n  operationId: documentVerificationVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/verifications/documenttypes/{countryCode}\n  method: get\n  operationId: getDocumentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/knownfaces/lists\n  method: get\n  operationId: getKnownFacesLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v3/knownfaces/lists\n  method: post\n  operationId: postKnownFacesList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/knownfaces/lists/{listId}\n  method: delete\n  operationId: deleteKnownFacesList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/knownfaces/lists/{listId}/transactions\n  method: get\n  operationId: getKnownFacesListTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v3/knownfaces/lists/{listId}/transactions\n  method: post\n  operationId: addKnownFacesListTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/check\n  method: post\n  operationId: personFraudCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/configuration/countrycodes/{configurationName}\n  method: get\n  operationId: getPersonFraudCountryCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /risk/v1/configuration/fields/{configurationName}/{countryCode}\n  method: get\n  operationId: getPersonFraudFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk/v1/configuration/datasources/{configurationName}/{countryCode}\n  method: get\n  operationId: getPersonFraudDatasources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/v2/auth/customer\n  method: post\n  operationId: postAuthCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/flow/{userStateId}\n  method: get\n  operationId: getFlow\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/v2/flow/{userStateId}\n  method: post\n  operationId: submitFlowData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/flow/{userStateId}/file\n  method: post\n  operationId: submitFlowFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/flow/{userStateId}/back\n  method: post\n  operationId: flowBack\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/handoff\n  method: post\n  operationId: postHandoff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/init\n  method: post\n  operationId: createOrUpdateUserState\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/workflows\n  method: get\n \
  \ operationId: getWorkflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/v2/profiles\n  method: get\n  operationId: getProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/v2/profiles/{clientId}\n  method: get\n  operationId: getProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/v2/profiles/{clientId}/file/{fileId}\n  method: get\n  operationId: getClientFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customer/v2/endclients/link\n  method: post\n  operationId: createLinkedLead\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/endclients/link\n  method: delete\n  operationId: deleteLinkedLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/endclients/bulkdelete\n  method: post\n  operationId: deleteEndClientsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/endclients/bulkstatus\n\
  \  method: post\n  operationId: updateEndClientsStatusBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/signedurl\n  method: post\n  operationId: generateSignedUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customer/v2/events\n  method: post\n  operationId: sendEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/verifications/verify\n  method: post\n  operationId: verifyPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/verifications/transactionrecord/{transactionRecordId}\n  method: get\n  operationId: getTransactionRecord\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/verifications/transactionrecord/{transactionRecordId}/withaddress\n  method: get\n  operationId: getTransactionRecordWithAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v3/verifications/transaction/{transactionId}/status\n  method: get\n  operationId: getTransactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/verifications/transaction/{transactionRecordId}/partialresult\n  method: get\n  operationId: getPartialTransactionResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/verifications/documentdownload/{transactionRecordId}/{fieldName}\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/agentic-access/trulioo-agentic-access.yml
summary_line: 54 operations · 20 acting
tags:
- Identity Verification
- KYC
- KYB
- AML
- Watchlist Screening
- Biometrics
- Document Verification
- Fraud Prevention
- Compliance
- Global Identity
---
