---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 9
api_specs:
- filename: volkswagen-catalog-api-openapi.yml
  format: yaml
  label: Volkswagen Catalog API
  slug: volkswagen-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volkswagen/refs/heads/main/openapi/volkswagen-catalog-api-openapi.yml
- filename: volkswagen-configuration-api-openapi.yml
  format: yaml
  label: Volkswagen Configuration API
  slug: volkswagen-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volkswagen/refs/heads/main/openapi/volkswagen-configuration-api-openapi.yml
- filename: volkswagen-information-api-openapi.yml
  format: yaml
  label: Volkswagen Information API
  slug: volkswagen-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/volkswagen/refs/heads/main/openapi/volkswagen-information-api-openapi.yml
consequence_counts:
  read: 9
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Volkswagen Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Volkswagen exposes 12 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Volkswagen
provider_slug: volkswagen
slug: volkswagen-agentic-access
source_filename: volkswagen-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/volkswagen-catalog-api-openapi.yml, openapi/volkswagen-configuration-api-openapi.yml,\n  openapi/volkswagen-information-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 9\n    acting: 3\n  by_consequence:\n    read: 9\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{countryCode}/brands\n  method: get\n  operationId: listBrandsByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{countryCode}/brands/{brandId}/models\n  method: get\n  operationId: listModelsByBrand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{countryCode}/models/{modelId}/types\n  method: get\n  operationId: listTypesByModel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{countryCode}/types/{typeId}/options\n  method: get\n  operationId: listOptionsByType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operation/{countryCode}/check\n  method: post\n  operationId: checkBuildability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/{countryCode}/recover\n  method: post\n  operationId: recoverConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/{countryCode}/configure\n  method: post\n  operationId: getConfigurationOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operation/{countryCode}/resolve\n  method: post\n  operationId: resolveConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /operation/{countryCode}/wltp\n  method: post\n  operationId: getWltpData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operation/{countryCode}/images\n  method: post\n  operationId: getConfigurationImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operation/{countryCode}/order\n  method: post\n  operationId: getOrderInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volkswagen/refs/heads/main/agentic-access/volkswagen-agentic-access.yml
summary_line: 12 operations · 3 acting
tags:
- Automobiles
- Cars
- Vehicles
- Automotive
- Vehicle Configuration
---
