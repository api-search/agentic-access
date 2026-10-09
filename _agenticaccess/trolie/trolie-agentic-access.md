---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 15
api_specs:
- filename: trolie-forecasting-api-openapi.yml
  format: yaml
  label: TROLIE Forecasting API
  slug: trolie-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-forecasting-api-openapi.yml
- filename: trolie-monitoring-sets-api-openapi.yml
  format: yaml
  label: TROLIE Monitoring Sets API
  slug: trolie-monitoring-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-monitoring-sets-api-openapi.yml
- filename: trolie-seasonal-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal API
  slug: trolie-seasonal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-api-openapi.yml
- filename: trolie-seasonal-overrides-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal Overrides API
  slug: trolie-seasonal-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-overrides-api-openapi.yml
- filename: trolie-temporary-aar-exceptions-api-openapi.yml
  format: yaml
  label: TROLIE Temporary AAR Exceptions API
  slug: trolie-temporary-aar-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-temporary-aar-exceptions-api-openapi.yml
- filename: trolie-realtime-api-openapi.yml
  format: yaml
  label: TROLIE Realtime API
  slug: trolie-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-realtime-api-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 3
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Trolie Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /seasonal-overrides
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /seasonal-overrides/{id}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /seasonal-overrides/{id}
operation_count: 28
overview: 'TROLIE exposes 28 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 10 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TROLIE
provider_slug: trolie
slug: trolie-agentic-access
source_filename: trolie-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/trolie-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    connected: 15\n    acting: 13\n  by_consequence:\n    read: 15\n    write: 10\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /limits/forecast-snapshot\n  method: get\n  operationId: getLimitsForecastSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:operating-snapshot\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /limits/forecast-snapshot/{period}\n  method: get\n  operationId: getHistoricalLimitsForecastSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - read:operating-snapshot\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /limits/regional/forecast-snapshot\n  method: get\n  operationId: getRegionalLimitsForecastSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:regional-operating-snapshot\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /limits/regional/forecast-snapshot\n  method: post\n  operationId: postRegionalLimitsForecastSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:regional-operating-snapshot\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rating-proposals/realtime\n  method: get\n  operationId: getRealTimeProposalStatus\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:realtime-proposals\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rating-proposals/realtime\n  method: post\n  operationId: postRealTimeProposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:realtime-proposals\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /limits/realtime-snapshot\n  method: get\n  operationId: getRealTimeLimits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:operating-snapshot\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /limits/regional/realtime-snapshot\n  method: get\n  operationId: getRegionalRealTimeLimits\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - read:operating-snapshot\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rating-proposals/forecast\n  method: get\n  operationId: getRatingForecastProposalStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:forecast-proposals\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rating-proposals/forecast\n  method: patch\n  operationId: patchRatingForecastProposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:forecast-proposals\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /seasonal-ratings/snapshot\n  method: get\n  operationId: getSeasonalRatingsSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    scope:\n    - read:operating-snapshot\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rating-proposals/seasonal\n  method: get\n  operationId: getSeasonalRatingProposalStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:seasonal-proposals\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rating-proposals/seasonal\n  method: patch\n  operationId: patchSeasonalRatingsProposal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:seasonal-proposals\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /seasonal-overrides\n  method: get\n  operationId: getSeasonalOverrides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - read:seasonal-overrides\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /seasonal-overrides\n  method: post\n  operationId: createSeasonalOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - write:seasonal-overrides\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /seasonal-overrides/{id}\n  method: get\n  operationId: getSeasonalOverride\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:seasonal-overrides\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /seasonal-overrides/{id}\n  method: delete\n  operationId: deleteSeasonalOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n\
  \    scope:\n    - write:seasonal-overrides\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /seasonal-overrides/{id}\n  method: put\n  operationId: updateSeasonalOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - write:seasonal-overrides\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /temporary-aar-exceptions\n  method: get\n  operationId: getTemporaryAARExceptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:temporary-aar-exceptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /temporary-aar-exceptions\n\
  \  method: post\n  operationId: createTemporaryAARException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:temporary-aar-exceptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /temporary-aar-exceptions/{id}\n  method: get\n  operationId: getTemporaryAARException\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:temporary-aar-exceptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /temporary-aar-exceptions/{id}\n  method: delete\n  operationId: deleteTemporaryAARException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:temporary-aar-exceptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /temporary-aar-exceptions/{id}\n  method: put\n  operationId: updateTemporaryAARException\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:temporary-aar-exceptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitoring-sets\n  method: post\n  operationId: createMonitoringSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:monitoring-sets\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitoring-sets/{id}\n  method: get\n  operationId: getMonitoringSet\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:monitoring-sets\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /monitoring-sets/{id}\n  method: put\n  operationId: updateMonitoringSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:monitoring-sets\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /monitoring-sets/{id}\n  method: delete\n  operationId: deleteMonitoringSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:monitoring-sets\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /default-monitoring-set\n\
  \  method: get\n  operationId: getDefaultMonitoringSet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:monitoring-sets\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/agentic-access/trolie-agentic-access.yml
summary_line: 28 operations · 13 acting · 3 human-in-the-loop
tags:
- Company
- Energy
- Electric Grid
- Transmission
- Open Standards
- OpenAPI
- LF Energy
- Open Source
---
