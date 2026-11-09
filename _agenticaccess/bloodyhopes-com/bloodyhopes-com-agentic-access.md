---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: bloodyhopes-com-campfire-api-openapi.yml
  format: yaml
  label: Bloody Hopes Campfire API
  slug: bloodyhopes-com-campfire-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloodyhopes-com/openapi/bloodyhopes-com-campfire-api-openapi.yml
- filename: bloodyhopes-com-growth-api-openapi.yml
  format: yaml
  label: Bloody Hopes Growth API
  slug: bloodyhopes-com-growth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloodyhopes-com/openapi/bloodyhopes-com-growth-api-openapi.yml
- filename: bloodyhopes-com-harness-api-openapi.yml
  format: yaml
  label: Bloody Hopes Harness API
  slug: bloodyhopes-com-harness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bloodyhopes-com/openapi/bloodyhopes-com-harness-api-openapi.yml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bloodyhopes Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Bloody Hopes exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bloody Hopes
provider_slug: bloodyhopes-com
slug: bloodyhopes-com-agentic-access
source_filename: bloodyhopes-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bloodyhopes-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 6\n    acting: 4\n  by_consequence:\n    read: 6\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/harness/tasks\n  method: get\n  operationId: listHarnessTasks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/harness/search\n  method: get\n  operationId: searchHarnessCorpus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/campfire\n\
  \  method: get\n  operationId: readCampfire\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/campfire/assignment\n  method: get\n  operationId: requestCriticalAssignment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/campfire/quick\n  method: post\n  operationId: leaveQuickVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/campfire/dry-run\n  method: post\n  operationId: validateCampfireVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/campfire/funnel\n  method: get\n  operationId: readAgentFunnel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/campfire/contributions\n  method: post\n  operationId: submitCampfireVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/growth/summary\n  method: get\n  operationId: readGrowthSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/campfire/vote\n  method: post\n  operationId:\
  \ upvoteVoice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/bloodyhopes-com/agentic-access/bloodyhopes-com-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Music
- Historical
- War
- Ballads
- AI-assisted
---
