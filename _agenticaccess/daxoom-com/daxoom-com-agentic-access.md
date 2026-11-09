---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 19
api_specs:
- filename: daxoom-com-analytics-api-openapi.yml
  format: yaml
  label: Daxoom Analytics API
  slug: daxoom-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-analytics-api-openapi.yml
- filename: daxoom-com-api-keys-api-openapi.yml
  format: yaml
  label: Daxoom API Keys API
  slug: daxoom-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-api-keys-api-openapi.yml
- filename: daxoom-com-businesses-api-openapi.yml
  format: yaml
  label: Daxoom Businesses API
  slug: daxoom-com-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-businesses-api-openapi.yml
- filename: daxoom-com-categories-api-openapi.yml
  format: yaml
  label: Daxoom Categories API
  slug: daxoom-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-categories-api-openapi.yml
- filename: daxoom-com-search-api-openapi.yml
  format: yaml
  label: Daxoom Search API
  slug: daxoom-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-search-api-openapi.yml
- filename: daxoom-com-system-api-openapi.yml
  format: yaml
  label: Daxoom System API
  slug: daxoom-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daxoom-com/openapi/daxoom-com-system-api-openapi.yml
consequence_counts:
  read: 19
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Daxoom Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/api_key/delete
operation_count: 23
overview: 'Daxoom exposes 23 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read, 3 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Daxoom
provider_slug: daxoom-com
slug: daxoom-com-agentic-access
source_filename: daxoom-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/daxoom-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 19\n    acting: 4\n  by_consequence:\n    read: 19\n    write: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /pubapi/v1/businesses\n  method: get\n  operationId: listBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/businesses/{id}\n  method: get\n  operationId: getBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /pubapi/v1/businesses/{id}/hours\n  method: get\n  operationId: getBusinessHours\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/businesses/{id}/offerings\n  method: get\n  operationId: getBusinessOfferings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/businesses/{id}/attributes\n  method: get\n  operationId: getBusinessAttributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/businesses/{id}/answers\n  method: get\n  operationId: getBusinessAnswers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/businesses/{id}/ai-context\n\
  \  method: get\n  operationId: getBusinessAIContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/search\n  method: get\n  operationId: semanticSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/services\n  method: get\n  operationId: searchServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubapi/v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v1/auth/login\n  method: post\n  operationId: authLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api_key/generate\n  method: post\n  operationId: generateApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api_key/roll\n  method: post\n  operationId: rollApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api_key/list\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api_key/delete\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/analytics/{businessId}/overview\n  method: get\n  operationId: getAnalyticsOverview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/{businessId}/queries\n\
  \  method: get\n  operationId: getAnalyticsQueries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/{businessId}/platforms\n  method: get\n  operationId: getAnalyticsPlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/{businessId}/trending\n  method: get\n  operationId: getAnalyticsTrending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/{businessId}/top-endpoints\n  method: get\n  operationId: getAnalyticsTopEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/{businessId}/reports\n \
  \ method: get\n  operationId: listVisibilityReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analytics/{businessId}/reports/{reportId}\n  method: get\n  operationId: getVisibilityReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/daxoom-com/agentic-access/daxoom-com-agentic-access.yml
summary_line: 23 operations · 4 acting · 1 human-in-the-loop
tags:
- Local Business Data
- AI Agents
- Verified Profiles
- POS Integration
- Analytics
---
