---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 12
api_specs:
- filename: whisper-online-a2a-api-openapi.yml
  format: yaml
  label: Whisper Security A2a API
  slug: whisper-online-a2a-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-a2a-api-openapi.yml
- filename: whisper-online-checkpoint-api-openapi.yml
  format: yaml
  label: Whisper Security Checkpoint API
  slug: whisper-online-checkpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-checkpoint-api-openapi.yml
- filename: whisper-online-consistency-api-openapi.yml
  format: yaml
  label: Whisper Security Consistency API
  slug: whisper-online-consistency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-consistency-api-openapi.yml
- filename: whisper-online-inclusion-api-openapi.yml
  format: yaml
  label: Whisper Security Inclusion API
  slug: whisper-online-inclusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-inclusion-api-openapi.yml
- filename: whisper-online-menu-api-openapi.yml
  format: yaml
  label: Whisper Security Menu API
  slug: whisper-online-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-menu-api-openapi.yml
- filename: whisper-online-query-api-openapi.yml
  format: yaml
  label: Whisper Security Query API
  slug: whisper-online-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-query-api-openapi.yml
- filename: whisper-online-tile-api-openapi.yml
  format: yaml
  label: Whisper Security Tile API
  slug: whisper-online-tile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-tile-api-openapi.yml
- filename: whisper-online-verify-identity-api-openapi.yml
  format: yaml
  label: Whisper Security Verify Identity API
  slug: whisper-online-verify-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-verify-identity-api-openapi.yml
- filename: whisper-online-well-known-api-openapi.yml
  format: yaml
  label: Whisper Security .well Known API
  slug: whisper-online-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-well-known-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Whisper Online Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /a2a
operation_count: 13
overview: 'Whisper Security exposes 13 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Whisper Security
provider_slug: whisper-online
slug: whisper-online-agentic-access
source_filename: whisper-online-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/whisper-online-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 12\n    acting: 1\n  by_consequence:\n    read: 12\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/query\n  method: post\n  operationId: query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /a2a\n  method: post\n  operationId: a2aSendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify-identity\n  method: get\n  operationId: verifyIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkpoint\n  method: get\n  operationId: ledgerCheckpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkpoint/key\n  method: get\n  operationId: ledgerCheckpointKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /checkpoint/status-list\n  method: get\n  operationId: ledgerStatusList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /checkpoint/ots/latest-confirmed\n  method: get\n  operationId: ledgerOtsLatestConfirmed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tile/{level}/{index}\n  method: get\n  operationId: ledgerTile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inclusion\n  method: get\n  operationId: ledgerInclusion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consistency\n  method: get\n  operationId: ledgerConsistency\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /menu\n  method: get\n  operationId: menu\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: agentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-onboarding.json\n  method: get\n  operationId: agentOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/agentic-access/whisper-online-agentic-access.yml
summary_line: 13 operations · 1 acting
tags:
- Agent Identity
- Agents
- IPv6
- DNS
- DNSSEC
- Threat Intelligence
- Security
- Egress
- A2A
- MCP
- RDAP
- Transparency Log
- Graph Database
- Agent-Native
- Netherlands
---
