---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: portscan-com-deep-api-openapi.yml
  format: yaml
  label: portscan-com Deep API
  slug: portscan-com-deep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/portscan-com/openapi/portscan-com-deep-api-openapi.yml
- filename: portscan-com-fast-api-openapi.yml
  format: yaml
  label: portscan-com Fast API
  slug: portscan-com-fast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/portscan-com/openapi/portscan-com-fast-api-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Portscan Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'portscan-com exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: portscan-com
provider_slug: portscan-com
slug: portscan-com-agentic-access
source_filename: portscan-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/portscan-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 2\n    connected: 4\n  by_consequence:\n    write: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/fast\n  method: post\n  operationId: startFastScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fast\n  method: get\n  operationId: pollFastScan\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deep\n  method: post\n  operationId: startDeepScan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/deep\n  method: get\n  operationId: pollDeepScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/fast\n  method: get\n  operationId: streamFastScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/deep\n  method: get\n  operationId: streamDeepScan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/portscan-com/agentic-access/portscan-com-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Networking
- Security
- Port Scanning
---
