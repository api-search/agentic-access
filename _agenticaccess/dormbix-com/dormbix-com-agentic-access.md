---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: dormbix-com-ai-feed-json-api-openapi.yml
  format: yaml
  label: DormBix Ai Feed.json API
  slug: dormbix-com-ai-feed-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dormbix-com/openapi/dormbix-com-ai-feed-json-api-openapi.yml
- filename: dormbix-com-public-api-openapi.yml
  format: yaml
  label: DormBix Public API
  slug: dormbix-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dormbix-com/openapi/dormbix-com-public-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dormbix Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'DormBix exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DormBix
provider_slug: dormbix-com
slug: dormbix-com-agentic-access
source_filename: dormbix-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dormbix-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/public/ai/search\n  method: get\n  operationId: searchDorms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/ai/availability\n  method: get\n  operationId: checkAvailability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/ai/availability\n\
  \  method: post\n  operationId: batchCheckAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/public/ai/dorm/{id}\n  method: get\n  operationId: getDormDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-feed.json\n  method: get\n  operationId: getVacancyFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dormbix-com/agentic-access/dormbix-com-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Dormitory Management
- Artificial Intelligence
- Billing Automation
- Thai Market
- Software-as-a-Service
---
