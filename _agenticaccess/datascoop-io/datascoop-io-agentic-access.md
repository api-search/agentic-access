---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 19
api_specs:
- filename: datascoop-io-australia-api-openapi.yml
  format: yaml
  label: DataScoop Australia API
  slug: datascoop-io-australia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-australia-api-openapi.yml
- filename: datascoop-io-datasets-api-openapi.yml
  format: yaml
  label: DataScoop Datasets API
  slug: datascoop-io-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-datasets-api-openapi.yml
- filename: datascoop-io-me-api-openapi.yml
  format: yaml
  label: DataScoop Me API
  slug: datascoop-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-me-api-openapi.yml
- filename: datascoop-io-pricing-api-openapi.yml
  format: yaml
  label: DataScoop Pricing API
  slug: datascoop-io-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-pricing-api-openapi.yml
- filename: datascoop-io-saved-care-territories-api-openapi.yml
  format: yaml
  label: DataScoop Saved care territories API
  slug: datascoop-io-saved-care-territories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-saved-care-territories-api-openapi.yml
- filename: datascoop-io-signup-api-openapi.yml
  format: yaml
  label: DataScoop Signup API
  slug: datascoop-io-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-signup-api-openapi.yml
- filename: datascoop-io-united-kingdom-api-openapi.yml
  format: yaml
  label: DataScoop United Kingdom API
  slug: datascoop-io-united-kingdom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-united-kingdom-api-openapi.yml
- filename: datascoop-io-united-states-api-openapi.yml
  format: yaml
  label: DataScoop United States API
  slug: datascoop-io-united-states-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datascoop-io/openapi/datascoop-io-united-states-api-openapi.yml
consequence_counts:
  read: 19
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Datascoop Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 24
overview: 'DataScoop exposes 24 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DataScoop
provider_slug: datascoop-io
slug: datascoop-io-agentic-access
source_filename: datascoop-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/datascoop-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    connected: 19\n    acting: 5\n  by_consequence:\n    read: 19\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/datasets\n  method: get\n  operationId: listDatasets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{id}\n  method: get\n  operationId: getDatasetSchema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/{id}/query\n\
  \  method: get\n  operationId: queryDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pricing\n  method: get\n  operationId: getPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signup\n  method: post\n  operationId: signup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/datasets/cqc/query\n  method: get\n  operationId: query_cqc\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/fsa/query\n  method: get\n  operationId: query_fsa\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/us-food-inspections/query\n  method: get\n  operationId: query_us_food_inspections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/us-building-permits/query\n  method: get\n  operationId: query_us_building_permits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/fhis-scotland/query\n  method: get\n  operationId: query_fhis_scotland\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/charity-commission/query\n  method: get\n  operationId: query_charity_commission\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/companies-house/query\n  method: get\n  operationId: query_companies_house\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/us-motor-carriers/query\n  method: get\n  operationId: query_us_motor_carriers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/us-business-licenses/query\n  method: get\n  operationId: query_us_business_licenses\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/us-liquor-licenses/query\n  method: get\n  operationId: query_us_liquor_licenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/au-aged-care/query\n  method: get\n  operationId: query_au_aged_care\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/cqc/intelligence\n  method: get\n  operationId: get_cqc_intelligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/care-territories\n  method: get\n  operationId: listCareTerritories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/care-territories\n  method: post\n  operationId: createCareTerritory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/care-territories/{id}\n  method: get\n  operationId: getCareTerritory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/care-territories/{id}\n  method: delete\n  operationId: deleteCareTerritory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/care-territories/{id}/check\n  method: post\n  operationId: checkCareTerritory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/care-territories/{id}/review\n  method: post\n  operationId: reviewCareTerritory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/datascoop-io/agentic-access/datascoop-io-agentic-access.yml
summary_line: 24 operations · 5 acting
tags:
- Data
- Public Records
- AI Agents
- Datasets
---
