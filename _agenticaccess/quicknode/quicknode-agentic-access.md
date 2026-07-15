---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 9
api_specs:
- filename: quicknode-asyncapi.yml
  format: yaml
  label: QuickNode Core RPC API
  slug: core-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/asyncapi/quicknode-asyncapi.yml
- filename: quicknode-streams-openapi.yml
  format: yaml
  label: QuickNode Streams
  slug: streams
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-streams-openapi.yml
- filename: quicknode-ipfs-openapi.yml
  format: yaml
  label: QuickNode IPFS API
  slug: ipfs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-ipfs-openapi.yml
- filename: quicknode-key-value-store-openapi.yml
  format: yaml
  label: QuickNode Key-Value Store
  slug: kv-store
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/openapi/quicknode-key-value-store-openapi.yml
consequence_counts:
  read: 9
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Quicknode Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'QuickNode exposes 22 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 13 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: QuickNode
provider_slug: quicknode
slug: quicknode-agentic-access
source_filename: quicknode-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/quicknode-ipfs-openapi.yml, openapi/quicknode-key-value-store-openapi.yml, openapi/quicknode-streams-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 13\n    connected: 9\n  by_consequence:\n    write: 13\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/s3/put-object\n  method: post\n  operationId: putObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pinning\n  method: get\n\
  \  operationId: listPins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pinning\n  method: post\n  operationId: pinByCid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pinning/{requestId}\n  method: get\n  operationId: getPin\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pinning/{requestId}\n  method: delete\n  operationId: deletePin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gateways\n  method: get\n  operationId: listGateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gateways\n  method: post\n  operationId: createGateway\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/account/usage\n  method: get\n  operationId: getAccountUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databases\n  method: get\n  operationId: listDatabases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databases\n  method: post\n  operationId: createDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /databases/{database}\n  method: delete\n  operationId: deleteDatabase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /databases/{database}/keys/{key}\n  method: get\n  operationId: getKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databases/{database}/keys/{key}\n\
  \  method: put\n  operationId: setKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /databases/{database}/keys/{key}\n  method: delete\n  operationId: deleteKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /databases/{database}/batch\n  method: post\n  operationId: batchWrite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    \
  \  - high-value\n    audit: required\n- path: /streams\n  method: get\n  operationId: listStreams\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams\n  method: post\n  operationId: createStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{streamId}\n  method: get\n  operationId: getStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /streams/{streamId}\n  method: delete\n  operationId: deleteStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{streamId}/pause\n  method: post\n  operationId: pauseStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{streamId}/resume\n  method: post\n  operationId: resumeStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /streams/{streamId}/logs\n  method: get\n  operationId: listStreamLogs\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quicknode/refs/heads/main/agentic-access/quicknode-agentic-access.yml
summary_line: 22 operations · 13 acting
tags:
- Web3
- Blockchain
- RPC
- Streams
- IPFS
- Multi-chain
---
