---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 14
api_specs:
- filename: aicdapi-com-agenda-hits-api-openapi.yml
  format: yaml
  label: aicdapi-com Agenda hits API
  slug: aicdapi-com-agenda-hits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-agenda-hits-api-openapi.yml
- filename: aicdapi-com-customer-civic-data-api-openapi.yml
  format: yaml
  label: aicdapi-com Customer civic data API
  slug: aicdapi-com-customer-civic-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-customer-civic-data-api-openapi.yml
- filename: aicdapi-com-data-reports-api-openapi.yml
  format: yaml
  label: aicdapi-com Data reports API
  slug: aicdapi-com-data-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-data-reports-api-openapi.yml
- filename: aicdapi-com-mcp-api-openapi.yml
  format: yaml
  label: aicdapi-com MCP API
  slug: aicdapi-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-mcp-api-openapi.yml
- filename: aicdapi-com-public-api-specification-api-openapi.yml
  format: yaml
  label: aicdapi-com Public API specification API
  slug: aicdapi-com-public-api-specification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-public-api-specification-api-openapi.yml
- filename: aicdapi-com-research-coverage-api-openapi.yml
  format: yaml
  label: aicdapi-com Research coverage API
  slug: aicdapi-com-research-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-research-coverage-api-openapi.yml
- filename: aicdapi-com-sources-api-openapi.yml
  format: yaml
  label: aicdapi-com Sources API
  slug: aicdapi-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-sources-api-openapi.yml
consequence_counts:
  read: 14
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Aicdapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/data/subscriptions/{subscriptionId}
operation_count: 21
overview: 'aicdapi-com exposes 21 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: aicdapi-com
provider_slug: aicdapi-com
slug: aicdapi-com-agentic-access
source_filename: aicdapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/aicdapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 7\n    connected: 14\n  by_consequence:\n    write: 6\n    read: 14\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/data/subscriptions\n  method: post\n  operationId: createFeedSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data/subscriptions\n  method: get\n  operationId: listFeedSubscriptions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/data/subscriptions/{subscriptionId}\n  method: delete\n  operationId: revokeFeedSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/data/subscriptions/{subscriptionId}/changes\n  method: get\n  operationId: readFeedSubscriptionChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: get\n  operationId: getPrelaunchMcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n \
  \   token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: postPrelaunchMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/openapi.json\n  method: get\n  operationId: getOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/mcp\n  method: post\n  operationId: postMcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data-reports\n  method:\
  \ post\n  operationId: submitDataReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data-reports/{reportId}\n  method: get\n  operationId: getDataReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/agenda-hits\n  method: get\n  operationId: listRecentAgendaHits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/agenda-hits/{matchId}\n  method: get\n  operationId: getAgendaHit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v1/public/upcoming-agenda-hits\n  method: get\n  operationId: listUpcomingAgendaHits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/source-status\n  method: get\n  operationId: listPublicSourceStatuses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/coverage\n  method: get\n  operationId: listDfwResearchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/public/jurisdictions/{slug}/bodies/{bodySlug}/cadence\n  method: get\n  operationId: getPublicBodyCadence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/data/snapshots\n  method: post\n  operationId: createCivicSnapshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data/snapshots/{snapshotId}/{resource}\n  method: get\n  operationId: readCivicSnapshotPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/data/changes\n  method: get\n  operationId: readCivicChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/data/batch\n  method: post\n  operationId: readCivicRecords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data/health\n  method: get\n  operationId: readCivicHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aicdapi-com/agentic-access/aicdapi-com-agentic-access.yml
summary_line: 21 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- Civic Data
- Government
- MCP
---
