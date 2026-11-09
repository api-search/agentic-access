---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 40
api_specs:
- filename: veldora-no-addresses-api-openapi.yml
  format: yaml
  label: veldora-no Addresses API
  slug: veldora-no-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-addresses-api-openapi.yml
- filename: veldora-no-alerts-api-openapi.yml
  format: yaml
  label: veldora-no Alerts API
  slug: veldora-no-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-alerts-api-openapi.yml
- filename: veldora-no-companies-api-openapi.yml
  format: yaml
  label: veldora-no Companies API
  slug: veldora-no-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-companies-api-openapi.yml
- filename: veldora-no-exchange-rates-api-openapi.yml
  format: yaml
  label: veldora-no Exchange Rates API
  slug: veldora-no-exchange-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-exchange-rates-api-openapi.yml
- filename: veldora-no-fi-api-openapi.yml
  format: yaml
  label: veldora-no Fi API
  slug: veldora-no-fi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-fi-api-openapi.yml
- filename: veldora-no-health-api-openapi.yml
  format: yaml
  label: veldora-no Health API
  slug: veldora-no-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-health-api-openapi.yml
- filename: veldora-no-laws-api-openapi.yml
  format: yaml
  label: veldora-no Laws API
  slug: veldora-no-laws-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-laws-api-openapi.yml
- filename: veldora-no-statistics-api-openapi.yml
  format: yaml
  label: veldora-no Statistics API
  slug: veldora-no-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-statistics-api-openapi.yml
- filename: veldora-no-tenders-api-openapi.yml
  format: yaml
  label: veldora-no Tenders API
  slug: veldora-no-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veldora-no/openapi/veldora-no-tenders-api-openapi.yml
consequence_counts:
  read: 40
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Veldora No Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 44
overview: 'veldora-no exposes 44 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: veldora-no
provider_slug: veldora-no
slug: veldora-no-agentic-access
source_filename: veldora-no-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/veldora-no-openapi.json, openapi/veldora-no-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    connected: 40\n    acting: 4\n  by_consequence:\n    read: 40\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/companies/{orgnr}\n  method: get\n  operationId: company\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies\n  method: get\n  operationId: companySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/companies/{orgnr}/tenders\n  method: get\n  operationId: companyTenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{orgnr}/awards\n  method: get\n  operationId: companyAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{orgnr}/units\n  method: get\n  operationId: companyUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenders\n  method: get\n  operationId: tenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts\n  method: post\n  operationId: alertCreate\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tenders/{id}\n  method: get\n  operationId: tender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses\n  method: get\n  operationId: addressSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses/nearby\n  method: get\n  operationId: addressesNearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/laws\n  method: get\n  operationId: lawSearch\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/laws/{id}\n  method: get\n  operationId: law\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/laws/{id}/sections/{section}\n  method: get\n  operationId: lawSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exchange-rates\n  method: get\n  operationId: exchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statistics/cpi\n  method: get\n  operationId: cpi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statistics/cpi/adjust\n  method: get\n  operationId:\
  \ cpiAdjust\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statistics/population\n  method: get\n  operationId: population\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fi/companies/{businessId}\n  method: get\n  operationId: fiCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fi/companies\n  method: get\n  operationId: fiCompanySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/{id}\n  method: get\n  operationId: getAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/{id}\n  method: delete\n  operationId: deleteAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{orgnr}\n  method: get\n  operationId: company\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies\n  method: get\n  operationId: companySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/companies/{orgnr}/tenders\n  method: get\n  operationId: companyTenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{orgnr}/awards\n  method: get\n  operationId: companyAwards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{orgnr}/units\n  method: get\n  operationId: companyUnits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tenders\n  method: get\n  operationId: tenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts\n  method: post\n  operationId: alertCreate\n  x-agentic-access:\n   \
  \ action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tenders/{id}\n  method: get\n  operationId: tender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses\n  method: get\n  operationId: addressSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses/nearby\n  method: get\n  operationId: addressesNearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/laws\n  method: get\n  operationId: lawSearch\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/laws/{id}\n  method: get\n  operationId: law\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/laws/{id}/sections/{section}\n  method: get\n  operationId: lawSection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exchange-rates\n  method: get\n  operationId: exchangeRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statistics/cpi\n  method: get\n  operationId: cpi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statistics/cpi/adjust\n  method:\
  \ get\n  operationId: cpiAdjust\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/statistics/population\n  method: get\n  operationId: population\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fi/companies/{businessId}\n  method: get\n  operationId: fiCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fi/companies\n  method: get\n  operationId: fiCompanySearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/{id}\n  method: get\n  operationId: getAlert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/{id}\n  method: delete\n  operationId: deleteAlert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/veldora-no/agentic-access/veldora-no-agentic-access.yml
summary_line: 44 operations · 4 acting
tags:
- Company
- Data
- Norway
- Artificial Intelligence
- Public Data
---
