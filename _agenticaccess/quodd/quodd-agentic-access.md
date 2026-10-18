---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: quodd-snapshots-api-openapi.yml
  format: yaml
  label: QUODD Snap API
  slug: quodd-snap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-snapshots-api-openapi.yml
- filename: quodd-snapshots-api-openapi.yml
  format: yaml
  label: QUODD Batch Snaps API
  slug: quodd-batch-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-snapshots-api-openapi.yml
- filename: quodd-options-api-openapi.yml
  format: yaml
  label: QUODD Options Snaps API
  slug: quodd-options-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-options-api-openapi.yml
- filename: quodd-authentication-api-openapi.yml
  format: yaml
  label: QUODD Authentication Token API
  slug: quodd-authentication-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/openapi/quodd-authentication-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Quodd Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'QUODD exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: QUODD
provider_slug: quodd
slug: quodd-agentic-access
source_filename: quodd-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/quodd-authentication-api-openapi.yml, openapi/quodd-options-api-openapi.yml,\n  openapi/quodd-snapshots-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 2\n    connected: 6\n  by_consequence:\n    write: 2\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /tokens/trial\n  method: post\n  operationId: createTrialToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokens/firm\n  method:\
  \ post\n  operationId: createFirmToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /options/snap/{ticker}\n  method: get\n  operationId: getOptionsSnap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/snaps\n  method: get\n  operationId: listOptionsSnaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/snaps\n  method: post\n  operationId: batchOptionsSnaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snap/{ticker}\n\
  \  method: get\n  operationId: getSnap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snaps\n  method: get\n  operationId: listSnaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /snaps\n  method: post\n  operationId: batchSnaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quodd/refs/heads/main/agentic-access/quodd-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- Market Data
- Real-Time Data
- Financial Data
- Streaming
- Historical Data
- Reference Data
- Quotes
- Fintech
---
