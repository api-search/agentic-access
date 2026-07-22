---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 4
api_specs:
- filename: subspace-openapi-original.yml
  format: yaml
  label: Subspace Product API
  slug: subspace-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/openapi/subspace-openapi-original.yml
consequence_counts:
  read: 4
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Subspace Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Subspace exposes 11 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Subspace
provider_slug: subspace
slug: subspace-agentic-access
source_filename: subspace-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/subspace-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 4\n    acting: 7\n  by_consequence:\n    read: 4\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/accelerator\n  method: get\n  operationId: AcceleratorService_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/accelerator\n  method: post\n  operationId: AcceleratorService_Create\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/accelerator/{id}\n  method: delete\n  operationId: AcceleratorService_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/accelerator/{id}\n  method: get\n  operationId: AcceleratorService_Get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/accelerator/{id}\n  method: put\n  operationId: AcceleratorService_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/sipteleport\n  method: get\n  operationId: SipTeleportService_List\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/sipteleport\n\
  \  method: post\n  operationId: SipTeleportService_Create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/sipteleport/{id}\n  method: delete\n  operationId: SipTeleportService_Delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/sipteleport/{id}\n  method: get\n  operationId: SipTeleportService_Get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/sipteleport/{id}\n  method: put\n  operationId: SipTeleportService_Update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n- path: /v1/webrtc-cdn\n  method: post\n  operationId: WebRtcCdnService_GetWebRtcCdn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - accelerators:read\n    - accelerators:write\n    - sipteleport:read\n    - sipteleport:write\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subspace/refs/heads/main/agentic-access/subspace-agentic-access.yml
summary_line: 11 operations · 7 acting
tags:
- Company
- Networking
- Real-Time
- WebRTC
- VoIP
- SIP
- CDN
- Gaming
- Latency
- Infrastructure
---
