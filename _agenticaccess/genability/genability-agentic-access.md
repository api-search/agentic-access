---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 30
api_specs:
- filename: genability-get-api-openapi.yml
  format: yaml
  label: Genability GET API
  slug: genability-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-get-api-openapi.yml
- filename: genability-rest-api-openapi.yml
  format: yaml
  label: Genability Rest API
  slug: genability-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-rest-api-openapi.yml
consequence_counts:
  read: 30
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Genability Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 33
overview: 'Genability exposes 33 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Genability
provider_slug: genability
slug: genability-agentic-access
source_filename: genability-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/genability-signal-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 33\n  by_action_class:\n    connected: 30\n    acting: 3\n  by_consequence:\n    read: 30\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /rest/echo/{error_code}\n  method: get\n  operationId: echo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/echo/hello\n  method: get\n  operationId: echo-api-hello\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/echo/errors\n\
  \  method: get\n  operationId: echo-api-errors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/echo/authenticate\n  method: get\n  operationId: echo-api-authenticate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/echo/validate\n  method: get\n  operationId: echo-api-validate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/ondemand/calculate\n  method: post\n  operationId: calculate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /rest/v1/ondemand/calculate/mass\n  method: post\n  operationId: mass-calculate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/prices/smart\n  method: get\n  operationId: smart-price-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/tariffs\n  method: get\n  operationId: get-tariff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/tariffs/{masterTariffId}/history\n  method: get\n  operationId: get-tariff-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/lses\n  method: get\n  operationId: get-lses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/lses/{lseId}\n  method: get\n  operationId: get-one-lse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/territories\n  method: get\n  operationId: territory-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/territories/{territoryId}\n  method: get\n  operationId: get-one-territory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/seasons\n  method: get\n\
  \  operationId: get-season\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/timeofuses/{lseId}/{touGroupId}\n  method: get\n  operationId: get-tou-group\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/timeofuses/{lseId}/{touGroupId}/intervals\n  method: get\n  operationId: get-tou-group-intervals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/timeofuses/{touId}\n  method: get\n  operationId: get-tou\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/timeofuses/intervals/{touId}\n  method: get\n  operationId: get-tou-intervals\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/timeofuses\n  method: post\n  operationId: tou-api-copy-3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/public/calendars/\n  method: get\n  operationId: get-calendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/calendars/{calendarId}\n  method: get\n  operationId: get-one-calendar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/calendars/dates\n \
  \ method: get\n  operationId: get-calendar-dates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/properties\n  method: get\n  operationId: properties-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/properties/{keyName}\n  method: get\n  operationId: get-one-property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /GET /rest/v1/utilitytaxes\n  method: get\n  operationId: get-utility-taxes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/utilitytaxes/{utilityTaxId}\n  method: get\n  operationId: get-one-utility-tax\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/properties/{keyName}/lookups\n  method: get\n  operationId: get-lookups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/properties/{propertyKey}/stats\n  method: get\n  operationId: lookup-stats-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/typicals/baselines/best\n  method: get\n  operationId: typical-baseline-api\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/zipcodes/{zipCode}\n  method: get\n  operationId: zip-code-api\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/orgs/usage\n  method: get\n  operationId: product-usage-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/public/tariffs/{masterTariffId}\n  method: get\n  operationId: get-tariff-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/agentic-access/genability-agentic-access.yml
summary_line: 33 operations · 3 acting
tags:
- Energy
- United States
- Utilities
- Electricity
- Tariffs
- Energy Rates
- Rate Calculation
- Energy Data Platform
- Solar
- Grid
---
