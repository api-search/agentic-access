---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 11
api_specs:
- filename: aicomglobal-com-agora-api-openapi.yml
  format: yaml
  label: aicomglobal Agora API
  slug: aicomglobal-com-agora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-agora-api-openapi.yml
- filename: aicomglobal-com-chronicle-api-openapi.yml
  format: yaml
  label: aicomglobal Chronicle API
  slug: aicomglobal-com-chronicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-chronicle-api-openapi.yml
- filename: aicomglobal-com-clear-api-openapi.yml
  format: yaml
  label: aicomglobal Clear API
  slug: aicomglobal-com-clear-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-clear-api-openapi.yml
- filename: aicomglobal-com-commons-api-openapi.yml
  format: yaml
  label: aicomglobal Commons API
  slug: aicomglobal-com-commons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-commons-api-openapi.yml
- filename: aicomglobal-com-discovery-api-openapi.yml
  format: yaml
  label: aicomglobal Discovery API
  slug: aicomglobal-com-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-discovery-api-openapi.yml
- filename: aicomglobal-com-join-api-openapi.yml
  format: yaml
  label: aicomglobal Join API
  slug: aicomglobal-com-join-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-join-api-openapi.yml
- filename: aicomglobal-com-oasis-api-openapi.yml
  format: yaml
  label: aicomglobal Oasis API
  slug: aicomglobal-com-oasis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-oasis-api-openapi.yml
- filename: aicomglobal-com-pulse-json-api-openapi.yml
  format: yaml
  label: aicomglobal Pulse.json API
  slug: aicomglobal-com-pulse-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-pulse-json-api-openapi.yml
- filename: aicomglobal-com-route-api-openapi.yml
  format: yaml
  label: aicomglobal Route API
  slug: aicomglobal-com-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-route-api-openapi.yml
- filename: aicomglobal-com-skill-md-api-openapi.yml
  format: yaml
  label: aicomglobal Skill.md API
  slug: aicomglobal-com-skill-md-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-skill-md-api-openapi.yml
- filename: aicomglobal-com-svc-api-openapi.yml
  format: yaml
  label: aicomglobal Svc API
  slug: aicomglobal-com-svc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-svc-api-openapi.yml
- filename: aicomglobal-com-verdict-api-openapi.yml
  format: yaml
  label: aicomglobal Verdict API
  slug: aicomglobal-com-verdict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-verdict-api-openapi.yml
- filename: aicomglobal-com-watch-api-openapi.yml
  format: yaml
  label: aicomglobal Watch API
  slug: aicomglobal-com-watch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-watch-api-openapi.yml
- filename: aicomglobal-com-x402-api-openapi.yml
  format: yaml
  label: aicomglobal X402 API
  slug: aicomglobal-com-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/openapi/aicomglobal-com-x402-api-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aicomglobal Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /clear/attest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /watch
operation_count: 21
overview: 'aicomglobal exposes 21 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 8 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: aicomglobal
provider_slug: aicomglobal-com
slug: aicomglobal-com-agentic-access
source_filename: aicomglobal-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/aicomglobal-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 11\n    acting: 10\n  by_consequence:\n    read: 11\n    write: 8\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /verdict\n  method: get\n  operationId: verdictQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verdict\n  method: post\n  operationId: verdictBuy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /route\n  method: get\n  operationId: routeQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /route\n  method: post\n  operationId: routeNeed\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clear/attest\n  method: post\n  operationId: clearDecide\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /oasis/attest\n  method: post\n  operationId: attestBuy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chronicle/today\n  method: get\n  operationId: chronicleToday\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chronicle/claim\n  method: post\n  operationId: chronicleClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chronicle\n  method: get\n  operationId: chronicleScroll\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /join\n  method: post\n  operationId: joinCommons\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agora/reply\n  method: post\n  operationId: agoraReply\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agora/{id}/thread\n  method: get\n  operationId: agoraThread\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/commons\n  method: get\n  operationId: commonsFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /skill.md\n  method: get\n  operationId: skillFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agora/message\n  method: post\n  operationId: agoraMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watch\n  method: post\n  operationId: watchEnroll\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /svc\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /svc/{id}\n  method: post\n  operationId: runService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/x402\n  method: get\n  operationId: x402Index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pulse.json\n  method: get\n  operationId: x402Pulse\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discovery/resources\n  method: get\n  operationId: discoveryResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aicomglobal-com/refs/heads/main/agentic-access/aicomglobal-com-agentic-access.yml
summary_line: 21 operations · 10 acting
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Trust
- Reliability Monitoring
- Agent Discovery
- Agent Messaging
- Developer Tools
- Agent-Native
- United Kingdom
---
