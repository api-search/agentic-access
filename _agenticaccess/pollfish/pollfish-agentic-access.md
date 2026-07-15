---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 14
api_specs:
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Apps API
  slug: pollfish-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Performance API
  slug: pollfish-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Revenue API
  slug: pollfish-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Respondent Demographics API
  slug: pollfish-respondent-demographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish User Logs API
  slug: pollfish-user-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Survey Distribution and Offerwall API
  slug: pollfish-survey-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Server-to-Server Callbacks
  slug: pollfish-s2s-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
consequence_counts:
  read: 14
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pollfish Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Pollfish exposes 17 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pollfish
provider_slug: pollfish
slug: pollfish-agentic-access
source_filename: pollfish-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pollfish-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 14\n    acting: 3\n  by_consequence:\n    read: 14\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/public/v2/apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v2/apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v2/apps/{api_key}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v2/apps/{api_key}\n  method: put\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/v2/apps/{api_key}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/public/v3/apps/performance\n  method: get\n  operationId: getAllAppsPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v3/apps/{api_key}/performance\n  method: get\n  operationId: getAppPerformance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v3/apps/{api_key}/performanceByCountry\n  method: get\n  operationId: getAppPerformanceByCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v3/apps/revenue\n  method: get\n  operationId: getAllAppsRevenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/public/v3/apps/{api_key}/revenue\n  method: get\n  operationId: getAppRevenue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v3/apps/revenuePerCountry\n  method: get\n  operationId: getAllAppsRevenuePerCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v3/apps/{api_key}/revenuePerCountry\n  method: get\n  operationId: getAppRevenuePerCountry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/v3/apps/demographics\n  method: get\n  operationId: getRespondentDemographics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/public/v3/apps/{api_key}/users_log\n  method: get\n  operationId: getUsersLog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/device/register/true\n  method: get\n  operationId: registerDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/device/register/true\n  method: head\n  operationId: checkSurveyAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/device/survey/{survey_id}\n  method: get\n  operationId: loadSurvey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/agentic-access/pollfish-agentic-access.yml
summary_line: 17 operations · 3 acting
tags:
- Surveys
- Market Research
- Mobile
- Monetization
- Offerwall
- Rewarded Ads
- Prodege
---
