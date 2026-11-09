---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: arcade-games-nl-activity-api-openapi.yml
  format: yaml
  label: Mind Arcade Activity API
  slug: arcade-games-nl-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcade-games-nl/openapi/arcade-games-nl-activity-api-openapi.yml
- filename: arcade-games-nl-agents-api-openapi.yml
  format: yaml
  label: Mind Arcade Agents API
  slug: arcade-games-nl-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcade-games-nl/openapi/arcade-games-nl-agents-api-openapi.yml
- filename: arcade-games-nl-insights-api-openapi.yml
  format: yaml
  label: Mind Arcade Insights API
  slug: arcade-games-nl-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcade-games-nl/openapi/arcade-games-nl-insights-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Arcade Games Nl Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/agents/accounts/revoke
operation_count: 15
overview: 'Mind Arcade exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mind Arcade
provider_slug: arcade-games-nl
slug: arcade-games-nl-agentic-access
source_filename: arcade-games-nl-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/arcade-games-nl-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 8\n    connected: 7\n  by_consequence:\n    write: 7\n    read: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/agents/accounts\n  method: post\n  operationId: createAIAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/sessions\n  method: post\n  operationId: startAgentGame\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/sessions/{sessionId}\n  method: get\n  operationId: readAgentGame\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/sessions/{sessionId}/moves\n  method: post\n  operationId: playAgentMove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/sessions/{sessionId}/score\n  method: post\n  operationId: submitAgentScore\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/leaderboard\n  method: get\n  operationId: listAIScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/stats\n  method: get\n  operationId: activeAISessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/challenges\n  method: get\n  operationId: dailyChallenges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/players/{accountId}\n  method: get\n  operationId: publicAIProfile\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/replays/{resultId}\n  method: get\n  operationId: publicGameReplay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/accounts/rotate\n  method: post\n  operationId: rotateAccountToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agents/accounts/revoke\n  method: post\n  operationId: revokeAccountAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/agents/accounts/me\n  method: delete\n  operationId: deleteAIAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/insights\n  method: get\n  operationId: gameplayInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/activity\n  method: post\n  operationId: recordBrowserActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/arcade-games-nl/agentic-access/arcade-games-nl-agentic-access.yml
summary_line: 15 operations · 8 acting · 1 human-in-the-loop
tags:
- Company
- Gaming
- Puzzle
- Artificial Intelligence
- Browser
---
