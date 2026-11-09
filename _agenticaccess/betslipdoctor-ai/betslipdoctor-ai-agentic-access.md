---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: betslipdoctor-ai-board-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Board API
  slug: betslipdoctor-ai-board-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-board-api-openapi.yml
- filename: betslipdoctor-ai-grade-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Grade API
  slug: betslipdoctor-ai-grade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-grade-api-openapi.yml
- filename: betslipdoctor-ai-history-api-openapi.yml
  format: yaml
  label: BetSlip Doctor History API
  slug: betslipdoctor-ai-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-history-api-openapi.yml
- filename: betslipdoctor-ai-reports-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Reports API
  slug: betslipdoctor-ai-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-reports-api-openapi.yml
- filename: betslipdoctor-ai-slips-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Slips API
  slug: betslipdoctor-ai-slips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-slips-api-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Betslipdoctor Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'BetSlip Doctor exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BetSlip Doctor
provider_slug: betslipdoctor-ai
slug: betslipdoctor-ai-agentic-access
source_filename: betslipdoctor-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/betslipdoctor-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/slips\n  method: get\n  operationId: getTrackedSlips\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - slips.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/slips\n  method: post\n  operationId: trackSlip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - slips.track\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/grade\n  method: post\n  operationId: gradeSlip\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - slips.grade\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/history\n  method: get\n  operationId: getHistorySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - history.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports\n  method: get\n  operationId: getSavedReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - reports.read\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/board\n  method: get\n  operationId: getBoard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - odds.read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/betslipdoctor-ai/agentic-access/betslipdoctor-ai-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Company
- Sports
- Betting
- Analytics
- Mobile
---
