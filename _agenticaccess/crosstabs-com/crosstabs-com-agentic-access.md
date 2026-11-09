---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 10
api_specs:
- filename: crosstabs-com-aggregate-statistics-api-openapi.yml
  format: yaml
  label: Crosstabs Aggregate statistics API
  slug: crosstabs-com-aggregate-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosstabs-com/openapi/crosstabs-com-aggregate-statistics-api-openapi.yml
- filename: crosstabs-com-chi-square-api-openapi.yml
  format: yaml
  label: Crosstabs Chi Square API
  slug: crosstabs-com-chi-square-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosstabs-com/openapi/crosstabs-com-chi-square-api-openapi.yml
- filename: crosstabs-com-contingency-api-openapi.yml
  format: yaml
  label: Crosstabs Contingency API
  slug: crosstabs-com-contingency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosstabs-com/openapi/crosstabs-com-contingency-api-openapi.yml
- filename: crosstabs-com-fishers-exact-api-openapi.yml
  format: yaml
  label: Crosstabs Fishers Exact API
  slug: crosstabs-com-fishers-exact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosstabs-com/openapi/crosstabs-com-fishers-exact-api-openapi.yml
- filename: crosstabs-com-odds-ratio-api-openapi.yml
  format: yaml
  label: Crosstabs Odds Ratio API
  slug: crosstabs-com-odds-ratio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosstabs-com/openapi/crosstabs-com-odds-ratio-api-openapi.yml
- filename: crosstabs-com-operations-api-openapi.yml
  format: yaml
  label: Crosstabs Operations API
  slug: crosstabs-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosstabs-com/openapi/crosstabs-com-operations-api-openapi.yml
consequence_counts:
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crosstabs Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Crosstabs exposes 14 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crosstabs
provider_slug: crosstabs-com
slug: crosstabs-com-agentic-access
source_filename: crosstabs-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/crosstabs-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 10\n    acting: 4\n  by_consequence:\n    read: 10\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/contingency\n  method: get\n  operationId: getContingency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/contingency\n  method: post\n  operationId: postContingency\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/contingency\n  method: options\n  operationId: optionsContingency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chi-square\n  method: get\n  operationId: getChiSquare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chi-square\n  method: post\n  operationId: postChiSquare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/chi-square\n  method: options\n  operationId: optionsChiSquare\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fishers-exact\n  method: get\n  operationId: getFishersExact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/fishers-exact\n  method: post\n  operationId: postFishersExact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/fishers-exact\n  method: options\n  operationId: optionsFishersExact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/odds-ratio\n  method: get\n  operationId: getOddsRatio\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/odds-ratio\n  method: post\n  operationId: postOddsRatio\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/odds-ratio\n  method: options\n  operationId: optionsOddsRatio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: head\n  operationId: headHealth\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/crosstabs-com/agentic-access/crosstabs-com-agentic-access.yml
summary_line: 14 operations · 4 acting
tags:
- Statistics
- Data Analysis
- Free Tools
- OpenAPI
- Browser-Based
---
