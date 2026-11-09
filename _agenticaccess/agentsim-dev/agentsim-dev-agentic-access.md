---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
api_specs:
- filename: agentsim-dev-agents-api-openapi.yml
  format: yaml
  label: AgentSIM Agents API
  slug: agentsim-dev-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-agents-api-openapi.yml
- filename: agentsim-dev-browser-access-api-openapi.yml
  format: yaml
  label: AgentSIM Browser Access API
  slug: agentsim-dev-browser-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-browser-access-api-openapi.yml
- filename: agentsim-dev-sessions-api-openapi.yml
  format: yaml
  label: AgentSIM Sessions API
  slug: agentsim-dev-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsim-dev/openapi/agentsim-dev-sessions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 5
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Agentsim Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /browser-connections/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sessions
operation_count: 13
overview: 'AgentSIM exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 6 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AgentSIM
provider_slug: agentsim-dev
slug: agentsim-dev-agentic-access
source_filename: agentsim-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentsim-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 8\n    connected: 5\n  by_consequence:\n    write: 6\n    physical: 1\n    read: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /agents/identify\n  method: post\n  operationId: identifyAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: post\n  operationId: provisionSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{id}/inject-email\n  method: post\n  operationId: injectEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{id}/wait\n  method: post\n  operationId: waitForOtp\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sessions/{id}/messages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browser-connections\n  method: post\n  operationId: createBrowserConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /browser-connections\n  method: get\n  operationId: listBrowserConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /browser-connections/{id}\n  method: get\n  operationId: getBrowserConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /browser-connections/{id}\n  method: delete\n  operationId: revokeBrowserConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sessions/{id}/resume\n  method: post\n  operationId: resumeBrowserAccess\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n \
  \     - high-value\n    audit: required\n- path: /sessions/{id}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sessions/{id}\n  method: delete\n  operationId: releaseSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentsim-dev/agentic-access/agentsim-dev-agentic-access.yml
summary_line: 13 operations · 8 acting · 1 human-in-the-loop
tags:
- AgentSIM
- Authentication
- Identity
- Security
---
