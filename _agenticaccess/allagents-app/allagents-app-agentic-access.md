---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: allagents-app-directory-api-openapi.yml
  format: yaml
  label: allagents Directory API
  slug: allagents-app-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allagents-app/refs/heads/main/openapi/allagents-app-directory-api-openapi.yml
- filename: allagents-app-discovery-api-openapi.yml
  format: yaml
  label: allagents Discovery API
  slug: allagents-app-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allagents-app/refs/heads/main/openapi/allagents-app-discovery-api-openapi.yml
- filename: allagents-app-listing-api-openapi.yml
  format: yaml
  label: allagents Listing API
  slug: allagents-app-listing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allagents-app/refs/heads/main/openapi/allagents-app-listing-api-openapi.yml
- filename: allagents-app-operator-api-openapi.yml
  format: yaml
  label: allagents Operator API
  slug: allagents-app-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allagents-app/refs/heads/main/openapi/allagents-app-operator-api-openapi.yml
consequence_counts:
  physical: 2
  read: 8
  safety-critical: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Allagents App Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /claim/verify
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /delist/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delist
operation_count: 16
overview: 'allagents exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 4 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: allagents
provider_slug: allagents-app
slug: allagents-app-agentic-access
source_filename: allagents-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: generated\nsource: openapi/allagents-app-directory-api-openapi.yml, openapi/allagents-app-discovery-api-openapi.yml,\n  openapi/allagents-app-listing-api-openapi.yml, openapi/allagents-app-operator-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 8\n    acting: 8\n  by_consequence:\n    read: 8\n    write: 4\n    safety-critical: 2\n    physical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /search\n  method: get\n  operationId: searchAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents\n  method: get\n  operationId: listAgents\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /category/{specialty}\n  method: get\n  operationId: listAgentsBySpecialty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/{slug}\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api\n  method: get\n  operationId: getApiIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /.well-known/agent-card.json\n  method: get\n  operationId: getAgentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update\n  method: post\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim\n  method: post\n  operationId: claimAgent\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claim/verify\n  method: post\n  operationId: verifyClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /delist\n  method: post\n  operationId: delistAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /delist/verify\n  method: post\n  operationId: verifyDelist\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /recover\n  method: post\n  operationId: recoverToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a\n  method: get\n  operationId: getA2aHint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a\n  method: post\n  operationId: a2aMessageSend\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allagents-app/refs/heads/main/agentic-access/allagents-app-agentic-access.yml
summary_line: 16 operations · 8 acting · 2 human-in-the-loop
tags:
- Company
- AI Agents
- Agent Directory
- A2A
- Discovery
- Search
- Registry
- Switzerland
---
