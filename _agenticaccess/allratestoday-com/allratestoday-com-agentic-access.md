---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 22
api_specs:
- filename: allratestoday-com-authentication-api-openapi.yml
  format: yaml
  label: allratestoday-com Authentication API
  slug: allratestoday-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-authentication-api-openapi.yml
- filename: allratestoday-com-central-bank-rates-api-openapi.yml
  format: yaml
  label: allratestoday-com Central Bank Rates API
  slug: allratestoday-com-central-bank-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-central-bank-rates-api-openapi.yml
- filename: allratestoday-com-compatibility-api-openapi.yml
  format: yaml
  label: allratestoday-com Compatibility API
  slug: allratestoday-com-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-compatibility-api-openapi.yml
- filename: allratestoday-com-market-rates-api-openapi.yml
  format: yaml
  label: allratestoday-com Market Rates API
  slug: allratestoday-com-market-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-market-rates-api-openapi.yml
- filename: allratestoday-com-open-endpoints-api-openapi.yml
  format: yaml
  label: allratestoday-com Open Endpoints API
  slug: allratestoday-com-open-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-open-endpoints-api-openapi.yml
- filename: allratestoday-com-reference-rate-api-openapi.yml
  format: yaml
  label: allratestoday-com Reference Rate API
  slug: allratestoday-com-reference-rate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allratestoday-com/openapi/allratestoday-com-reference-rate-api-openapi.yml
consequence_counts:
  read: 22
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Allratestoday Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'allratestoday-com exposes 23 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 22 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: allratestoday-com
provider_slug: allratestoday-com
slug: allratestoday-com-agentic-access
source_filename: allratestoday-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 22\n    acting: 1\n  by_consequence:\n    read: 22\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/rate\n  method: get\n  operationId: getRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/historical-rates\n  method: get\n  operationId: getHistoricalRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/rates\n  method: get\n  operationId:\
  \ getRatesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/symbols\n  method: get\n  operationId: getSymbols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/central-banks\n  method: get\n  operationId: listCentralBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/central-banks/rates\n  method: get\n  operationId: compareCentralBankRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/central-bank/{bank}/latest\n  method: get\n  operationId: getCentralBankLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/central-bank/{bank}/{date}\n  method: get\n  operationId: getCentralBankByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/central-bank/{bank}/history\n  method: get\n  operationId: getCentralBankHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/central-bank/{bank}/availability\n  method: get\n  operationId: getCentralBankAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open/central-banks\n  method: get\n  operationId: listOpenCentralBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/open/central-bank/{bank}\n  method: get\n  operationId: getOpenCentralBankLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/central-bank/{bank}\n  method: get\n  operationId: downloadCentralBankLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/open/geo\n  method: get\n  operationId: getVisitorGeo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/central-bank/{bank}/history\n  method: get\n  operationId: downloadCentralBankHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/compat/{provider}/latest\n\
  \  method: get\n  operationId: compatLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/compat/{provider}/{path}\n  method: get\n  operationId: compatDatedOrRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/keys\n  method: get\n  operationId: describeTrialKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/keys\n  method: post\n  operationId: issueTrialKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/open/reference-rate\n  method: get\n  operationId: getOpenReferenceRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reference-rate/latest\n  method: get\n  operationId: getReferenceRateLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reference-rate/{date}\n  method: get\n  operationId: getReferenceRateByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reference-rate/history\n  method: get\n  operationId: getReferenceRateHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/allratestoday-com/agentic-access/allratestoday-com-agentic-access.yml
summary_line: 23 operations · 1 acting
tags:
- Company
- Fintech
- Exchange Rates
- Data
---
