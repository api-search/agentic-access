---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: swisscom-process-create-api-openapi.yml
  format: yaml
  label: 'Swisscom Process: create API'
  slug: swisscom-process-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-process-create-api-openapi.yml
- filename: swisscom-process-read-api-openapi.yml
  format: yaml
  label: 'Swisscom Process: read API'
  slug: swisscom-process-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-process-read-api-openapi.yml
- filename: swisscom-signatures-api-openapi.yml
  format: yaml
  label: Swisscom Signatures API
  slug: swisscom-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/openapi/swisscom-signatures-api-openapi.yml
consequence_counts:
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Swisscom Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Swisscom exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Swisscom
provider_slug: swisscom
slug: swisscom-agentic-access
source_filename: swisscom-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: generated\nsource: openapi/swisscom-all-in-signing-service-openapi.yml, openapi/swisscom-sign-integration-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 6\n    connected: 6\n  by_consequence:\n    write: 6\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /signatures/signDoc\n  method: post\n  operationId: signDoc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/process\n  method: get\n  operationId:\
  \ findAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sswp:process:read:all\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/process\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sswp:process:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/process/{processId}/setup\n  method: post\n  operationId: setup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sswp:process:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/process/{processId}/release\n\
  \  method: post\n  operationId: release\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sswp:process:create\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/process/{processId}/open/{personId}\n  method: post\n  operationId: open\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sswp:process:read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/process/{processId}/attach\n  method: post\n  operationId: attach\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - sswp:process:create\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/process/{processId}\n  method: get\n  operationId: getProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sswp:process:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/process/{processId}/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sswp:process:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/process/{processId}/record\n  method: get\n  operationId: getRecords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sswp:process:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/process/{processId}/file/{fileId}\n  method:\
  \ get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sswp:process:read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/process/{processId}/file/{fileId}/content\n  method: get\n  operationId: getFileContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - sswp:process:read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swisscom/refs/heads/main/agentic-access/swisscom-agentic-access.yml
summary_line: 12 operations · 6 acting
tags:
- Telecommunications
- Switzerland
- Mobile Network Operator
- Broadband
- Network APIs
- Open Gateway
- Messaging
- SMS
- Voice
- Identity Verification
- Mobility Data
- Digital Signatures
- eSIM
- Artificial Intelligence
---
