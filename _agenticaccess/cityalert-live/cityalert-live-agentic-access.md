---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 10
api_specs:
- filename: cityalert-live-agents-api-openapi.yml
  format: yaml
  label: CityAlert.live Agents API
  slug: cityalert-live-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-agents-api-openapi.yml
- filename: cityalert-live-community-api-openapi.yml
  format: yaml
  label: CityAlert.live Community API
  slug: cityalert-live-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-community-api-openapi.yml
- filename: cityalert-live-feeds-api-openapi.yml
  format: yaml
  label: CityAlert.live Feeds API
  slug: cityalert-live-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-feeds-api-openapi.yml
- filename: cityalert-live-history-api-openapi.yml
  format: yaml
  label: CityAlert.live History API
  slug: cityalert-live-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-history-api-openapi.yml
- filename: cityalert-live-incidents-api-openapi.yml
  format: yaml
  label: CityAlert.live Incidents API
  slug: cityalert-live-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-incidents-api-openapi.yml
- filename: cityalert-live-meta-api-openapi.yml
  format: yaml
  label: CityAlert.live Meta API
  slug: cityalert-live-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-meta-api-openapi.yml
- filename: cityalert-live-news-api-openapi.yml
  format: yaml
  label: CityAlert.live News API
  slug: cityalert-live-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cityalert-live/openapi/cityalert-live-news-api-openapi.yml
consequence_counts:
  read: 10
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cityalert Live Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'CityAlert.live exposes 15 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CityAlert.live
provider_slug: cityalert-live
slug: cityalert-live-agentic-access
source_filename: cityalert-live-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cityalert-live-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 10\n    acting: 5\n  by_consequence:\n    read: 10\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/incidents\n  method: get\n  operationId: listIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/archive\n  method: get\n  operationId: queryArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/regions\n  method: get\n\
  \  operationId: listRegions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/trends\n  method: get\n  operationId: getTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/crime-year\n  method: get\n  operationId: getCrimeYear\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/news\n  method: get\n  operationId: listNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/reports\n  method: get\n  operationId: listReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /api/reports\n  method: post\n  operationId: createReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/reports/{id}/vote\n  method: post\n  operationId: voteReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dashboards\n  method: get\n  operationId: getDashboard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/dashboards\n  method: post\n  operationId: createDashboard\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/dashboards\n  method: put\n  operationId: updateDashboard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: post\n  operationId: mcpRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cities/{slug}/feed.xml\n  method:\
  \ get\n  operationId: cityFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openapi.json\n  method: get\n  operationId: openapiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cityalert-live/agentic-access/cityalert-live-agentic-access.yml
summary_line: 15 operations · 5 acting
tags:
- Safety
- Mapping
- Real-Time
- Open Data
- Community
---
