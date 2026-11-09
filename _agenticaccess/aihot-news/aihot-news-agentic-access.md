---
acting_count: 0
action_class_counts:
  connected: 25
api_specs:
- filename: aihot-news-agent-api-openapi.yml
  format: yaml
  label: AIHOT Agent API
  slug: aihot-news-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-agent-api-openapi.yml
- filename: aihot-news-dailies-api-openapi.yml
  format: yaml
  label: AIHOT Dailies API
  slug: aihot-news-dailies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-dailies-api-openapi.yml
- filename: aihot-news-hot-topics-api-openapi.yml
  format: yaml
  label: AIHOT Hot Topics API
  slug: aihot-news-hot-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-hot-topics-api-openapi.yml
- filename: aihot-news-items-api-openapi.yml
  format: yaml
  label: AIHOT Items API
  slug: aihot-news-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-items-api-openapi.yml
- filename: aihot-news-monthlies-api-openapi.yml
  format: yaml
  label: AIHOT Monthlies API
  slug: aihot-news-monthlies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-monthlies-api-openapi.yml
- filename: aihot-news-selected-api-openapi.yml
  format: yaml
  label: AIHOT Selected API
  slug: aihot-news-selected-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-selected-api-openapi.yml
- filename: aihot-news-stories-api-openapi.yml
  format: yaml
  label: AIHOT Stories API
  slug: aihot-news-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-stories-api-openapi.yml
- filename: aihot-news-weeklies-api-openapi.yml
  format: yaml
  label: AIHOT Weeklies API
  slug: aihot-news-weeklies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aihot-news/openapi/aihot-news-weeklies-api-openapi.yml
consequence_counts:
  read: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aihot News Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 25
overview: 'AIHOT exposes 25 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AIHOT
provider_slug: aihot-news
slug: aihot-news-agentic-access
source_filename: aihot-news-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/aihot-news-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 25\n  by_consequence:\n    read: 25\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/items\n  method: get\n  operationId: items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hot-topics\n  method: get\n  operationId: hotTopics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stories/{publicId}\n  method: get\n  operationId: storyByPublicId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dailies\n  method: get\n  operationId: dailies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dailies/latest\n  method: get\n  operationId: latestDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/dailies/{date}\n  method: get\n  operationId: dailyByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/weeklies\n  method: get\n  operationId: weeklies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/weeklies/latest\n  method: get\n  operationId: latestWeekly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/weeklies/{week}\n  method: get\n  operationId: weeklyByWeek\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monthlies\n  method: get\n  operationId: monthlies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monthlies/latest\n  method: get\n  operationId: latestMonthly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/monthlies/{month}\n  method: get\n  operationId: monthlyByMonth\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/selected/snapshot\n  method: get\n  operationId: selectedSnapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/selected/changes\n  method: get\n  operationId: selectedChanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent\n  method: get\n  operationId: agentGuide\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/latest\n  method: get\n  operationId: agentLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/v1/agent/search\n  method: get\n  operationId: agentSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/hot\n  method: get\n  operationId: agentHot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/stories/{publicId}\n  method: get\n  operationId: agentStory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/daily\n  method: get\n  operationId: agentLatestDaily\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/daily/{date}\n  method: get\n  operationId: agentDaily\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/weekly\n  method: get\n  operationId: agentWeekly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/weekly/{week}\n  method: get\n  operationId: agentWeeklyByWeek\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/monthly\n  method: get\n  operationId: agentMonthly\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/agent/monthly/{month}\n  method: get\n  operationId: agentMonthlyByMonth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aihot-news/agentic-access/aihot-news-agentic-access.yml
summary_line: 25 operations
tags:
- Company
---
