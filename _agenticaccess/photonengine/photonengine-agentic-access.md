---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 1
api_specs:
- filename: photonengine-asyncapi.yml
  format: yaml
  label: Photon Realtime Transport Protocol
  slug: photonengine-realtime-transport-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/asyncapi/photonengine-asyncapi.yml
- filename: photonengine-openapi.yml
  format: yaml
  label: Photon Room Lifecycle WebHooks
  slug: photonengine-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/openapi/photonengine-openapi.yml
- filename: photonengine-openapi.yml
  format: yaml
  label: Photon Custom Authentication Webservice Contract
  slug: photonengine-custom-authentication-webservice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/openapi/photonengine-openapi.yml
consequence_counts:
  read: 1
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Photonengine Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /BeforeJoin
operation_count: 8
overview: 'Photon Engine exposes 8 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Photon Engine
provider_slug: photonengine
slug: photonengine-agentic-access
source_filename: photonengine-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/photonengine-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 7\n    connected: 1\n  by_consequence:\n    write: 6\n    safety-critical: 1\n    read: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /Create\n  method: post\n  operationId: handlePathCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /BeforeJoin\n  method: post\n  operationId: handlePathBeforeJoin\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /Join\n  method: post\n  operationId: handlePathJoin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Leave\n  method: post\n  operationId: handlePathLeave\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Event\n  method: post\n  operationId:\
  \ handlePathEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /GameProperties\n  method: post\n  operationId: handlePathGameProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Close\n  method: post\n  operationId: handlePathClose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /CustomAuth\n  method: get\n  operationId: handleCustomAuthentication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photonengine/refs/heads/main/agentic-access/photonengine-agentic-access.yml
summary_line: 8 operations · 7 acting · 1 human-in-the-loop
tags:
- Gaming
- Multiplayer
- Realtime
- Netcode
- Game Networking
- WebSocket
- Binary Protocol
---
