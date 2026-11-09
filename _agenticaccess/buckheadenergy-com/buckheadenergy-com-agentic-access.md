---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: buckheadenergy-com-counties-api-openapi.yml
  format: yaml
  label: Buckhead Energy Counties API
  slug: buckheadenergy-com-counties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckheadenergy-com/openapi/buckheadenergy-com-counties-api-openapi.yml
- filename: buckheadenergy-com-encyclopedia-api-openapi.yml
  format: yaml
  label: Buckhead Energy Encyclopedia API
  slug: buckheadenergy-com-encyclopedia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckheadenergy-com/openapi/buckheadenergy-com-encyclopedia-api-openapi.yml
- filename: buckheadenergy-com-formations-api-openapi.yml
  format: yaml
  label: Buckhead Energy Formations API
  slug: buckheadenergy-com-formations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckheadenergy-com/openapi/buckheadenergy-com-formations-api-openapi.yml
- filename: buckheadenergy-com-operator-county-api-openapi.yml
  format: yaml
  label: Buckhead Energy Operator County API
  slug: buckheadenergy-com-operator-county-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckheadenergy-com/openapi/buckheadenergy-com-operator-county-api-openapi.yml
- filename: buckheadenergy-com-operators-api-openapi.yml
  format: yaml
  label: Buckhead Energy Operators API
  slug: buckheadenergy-com-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckheadenergy-com/openapi/buckheadenergy-com-operators-api-openapi.yml
- filename: buckheadenergy-com-payors-api-openapi.yml
  format: yaml
  label: Buckhead Energy Payors API
  slug: buckheadenergy-com-payors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckheadenergy-com/openapi/buckheadenergy-com-payors-api-openapi.yml
- filename: buckheadenergy-com-state-api-openapi.yml
  format: yaml
  label: Buckhead Energy State API
  slug: buckheadenergy-com-state-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckheadenergy-com/openapi/buckheadenergy-com-state-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buckheadenergy Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Buckhead Energy exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Buckhead Energy
provider_slug: buckheadenergy-com
slug: buckheadenergy-com-agentic-access
source_filename: buckheadenergy-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buckheadenergy-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/top\n  method: get\n  operationId: getNationalTopOperators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{slug}\n  method: get\n  operationId: getOperatorProfile\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /us-drilling-activity-index\n  method: get\n  operationId: getUsDrillingActivityIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/snapshot\n  method: get\n  operationId: getStateSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/operators\n  method: get\n  operationId: getTopOperators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/counties\n  method: get\n  operationId: getCountyDrillingActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/activity\n  method: get\n  operationId: getStateActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/cycle-times\n  method: get\n  operationId: getCycleTimes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/duc-aging\n  method: get\n  operationId: getDucAging\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/lateral-trends\n  method: get\n  operationId: getLateralTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/production-bands\n\
  \  method: get\n  operationId: getProductionBands\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /state/{state}/momentum\n  method: get\n  operationId: getStateMomentum\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counties/{state}/{county}/metrics\n  method: get\n  operationId: getCountyMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operator-county/stats\n  method: get\n  operationId: getOperatorCountyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operator-county/footprint\n  method: get\n  operationId: getOperatorCountyFootprint\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /formations/{state}/{slug}\n  method: get\n  operationId: getFormationDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payors\n  method: get\n  operationId: searchPayors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encyclopedia\n  method: get\n  operationId: getEncyclopediaTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /encyclopedia/{slug}\n  method: get\n  operationId: getEncyclopediaTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n"
source_yaml_url: https://artifacts.apis.io/buckheadenergy-com/agentic-access/buckheadenergy-com-agentic-access.yml
summary_line: 20 operations
tags:
- Energy
- Mineral Rights
- Oil and Gas
- Real Estate
- Texas
---
