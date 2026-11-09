---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 32
api_specs:
- filename: didlogic-com-account-balance-api-openapi.yml
  format: yaml
  label: DID Logic Account Balance API
  slug: didlogic-com-account-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-account-balance-api-openapi.yml
- filename: didlogic-com-api-access-api-openapi.yml
  format: yaml
  label: DID Logic API Access API
  slug: didlogic-com-api-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-api-access-api-openapi.yml
- filename: didlogic-com-calls-api-openapi.yml
  format: yaml
  label: DID Logic Calls API
  slug: didlogic-com-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-calls-api-openapi.yml
- filename: didlogic-com-click2call-api-openapi.yml
  format: yaml
  label: DID Logic Click2 Call API
  slug: didlogic-com-click2call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-click2call-api-openapi.yml
- filename: didlogic-com-hlr-lookups-api-openapi.yml
  format: yaml
  label: DID Logic HLR Lookups API
  slug: didlogic-com-hlr-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-hlr-lookups-api-openapi.yml
- filename: didlogic-com-identities-api-openapi.yml
  format: yaml
  label: DID Logic Identities API
  slug: didlogic-com-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-identities-api-openapi.yml
- filename: didlogic-com-inbound-destinations-api-openapi.yml
  format: yaml
  label: DID Logic Inbound Destinations API
  slug: didlogic-com-inbound-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-inbound-destinations-api-openapi.yml
- filename: didlogic-com-kyc-documents-api-openapi.yml
  format: yaml
  label: DID Logic KYC Documents API
  slug: didlogic-com-kyc-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-kyc-documents-api-openapi.yml
- filename: didlogic-com-numbers-inventory-api-openapi.yml
  format: yaml
  label: DID Logic Numbers & Inventory API
  slug: didlogic-com-numbers-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-numbers-inventory-api-openapi.yml
- filename: didlogic-com-purchases-api-openapi.yml
  format: yaml
  label: DID Logic Purchases API
  slug: didlogic-com-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-purchases-api-openapi.yml
- filename: didlogic-com-reports-api-openapi.yml
  format: yaml
  label: DID Logic Reports API
  slug: didlogic-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-reports-api-openapi.yml
- filename: didlogic-com-risk-checks-api-openapi.yml
  format: yaml
  label: DID Logic Risk Checks API
  slug: didlogic-com-risk-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-risk-checks-api-openapi.yml
- filename: didlogic-com-sip-accounts-api-openapi.yml
  format: yaml
  label: DID Logic SIP Accounts API
  slug: didlogic-com-sip-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-sip-accounts-api-openapi.yml
- filename: didlogic-com-sms-api-openapi.yml
  format: yaml
  label: DID Logic SMS API
  slug: didlogic-com-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-sms-api-openapi.yml
consequence_counts:
  physical: 7
  read: 32
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Didlogic Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/purchases/{purchase_id}/destinations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /api/v1/purchases/{purchase_id}/destinations/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/purchases/{purchase_id}/destinations/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/sms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/numbers/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v2/numbers/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v2/numbers/purchase
operation_count: 53
overview: 'DID Logic exposes 53 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 14 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DID Logic
provider_slug: didlogic-com
slug: didlogic-com-agentic-access
source_filename: didlogic-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/didlogic-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 53\n  by_action_class:\n    connected: 32\n    acting: 21\n  by_consequence:\n    read: 32\n    write: 14\n    physical: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/capabilities\n  method: get\n  operationId: capabilities_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/balance\n  method: get\n  operationId: balance_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/calls\n  method: get\n  operationId: calls_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calls/statistics\n  method: get\n  operationId: calls_statistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/calls/recording/{callid}\n  method: get\n  operationId: calls_recording\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/call_price\n  method: get\n  operationId: call_price_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/click2call\n  method: post\n  operationId: click2call_create\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/click2call/{id}\n  method: get\n  operationId: click2call_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/click2call/{id}\n  method: delete\n  operationId: click2call_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/recordings/{user_id}/{token}\n  method: get\n  operationId: recordings_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/asr_report\n  method: get\n  operationId: asr_report_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions\n  method: get\n  operationId: transactions_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/purchases\n  method: get\n  operationId: purchases_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/purchases/{purchase_id}/destinations\n  method: get\n  operationId: purchases_destinations_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/purchases/{purchase_id}/destinations\n\
  \  method: post\n  operationId: purchases_destinations_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/purchases/{purchase_id}/destinations/{id}\n  method: patch\n  operationId: purchases_destinations_update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/purchases/{purchase_id}/destinations/{id}\n  method: delete\n  operationId: purchases_destinations_destroy\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sipaccounts\n  method: get\n  operationId: sipaccounts_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sipaccounts\n  method: post\n  operationId: sipaccounts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sipaccounts/{id}\n  method: get\n  operationId: sipaccounts_show\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sipaccounts/{id}\n  method: patch\n  operationId: sipaccounts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sipaccounts/{id}\n  method: delete\n  operationId: sipaccounts_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sipaccounts/{sipaccount_id}/allowed_ips\n  method: get\n  operationId: sipaccounts_allowed_ips_index\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sipaccounts/{sipaccount_id}/allowed_ips\n  method: post\n  operationId: sipaccounts_allowed_ips_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sipaccounts/{sipaccount_id}/allowed_ips\n  method: delete\n  operationId: sipaccounts_allowed_ips_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sms\n  method: get\n  operationId: sms_index\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sms\n  method: post\n  operationId: sms_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sms/{id}\n  method: get\n  operationId: sms_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers/countries\n  method: get\n  operationId: numbers_countries_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers/countries/{country_id}/cities\n  method: get\n  operationId:\
  \ numbers_countries_cities_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers/countries/{country_id}/regions\n  method: get\n  operationId: numbers_countries_regions_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers/countries/{country_id}/locations\n  method: get\n  operationId: numbers_countries_locations_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers/countries/{country_id}/cities/{city_id}/dids\n  method: get\n  operationId: numbers_countries_cities_dids_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v2/numbers/search\n  method: get\n  operationId: numbers_search_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers\n  method: get\n  operationId: numbers_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers/purchase\n  method: post\n  operationId: numbers_purchase_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/numbers/purchase\n  method: put\n  operationId: numbers_purchase_update\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/numbers/purchase\n  method: delete\n  operationId: numbers_purchase_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/numbers/risk_checks\n  method: get\n  operationId: numbers_risk_checks_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/numbers/risk_checks\n  method: post\n\
  \  operationId: numbers_risk_checks_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/numbers/risk_checks/logs\n  method: get\n  operationId: numbers_risk_checks_logs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/hlr\n  method: post\n  operationId: hlr_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/hlr/history\n  method: get\n  operationId: hlr_history\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/documents\n  method: get\n  operationId: documents_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/documents\n  method: post\n  operationId: documents_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/documents/{id}\n  method: get\n  operationId: documents_show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/documents/{id}\n  method: put\n  operationId: documents_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/documents/{id}\n  method: delete\n  operationId: documents_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/documents/countries\n  method: get\n  operationId: documents_countries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/documents/{id}/files/{role}\n  method: get\n  operationId: documents_files_download_file\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identities\n  method: get\n  operationId: identities_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/identities\n  method: post\n  operationId: identities_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/identities/{id}\n  method: delete\n  operationId: identities_destroy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/didlogic-com/agentic-access/didlogic-com-agentic-access.yml
summary_line: 53 operations · 21 acting
tags:
- Company
- Telecommunications
- VoIP
- SIP Trunking
- DID Numbers
- SMS
- Voice
- MCP
---
