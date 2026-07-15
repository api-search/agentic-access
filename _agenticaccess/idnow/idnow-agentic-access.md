---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 1
api_specs:
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow Identifications API
  slug: idnow-identifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow Results & Retrieval API
  slug: idnow-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow AutoIdent API
  slug: idnow-autoident-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow VideoIdent API
  slug: idnow-videoident-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
- filename: idnow-openapi.yml
  format: yaml
  label: IDnow Webhooks
  slug: idnow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/openapi/idnow-openapi.yml
consequence_counts:
  read: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Idnow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'IDnow exposes 5 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: IDnow
provider_slug: idnow
slug: idnow-agentic-access
source_filename: idnow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/idnow-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 4\n    connected: 1\n  by_consequence:\n    write: 4\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /{company}/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{company}/identifications/{transactionId}/create\n  method: post\n  operationId: createIdentification\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{company}/identifications/{transactionId}/start\n  method: post\n  operationId: startIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{company}/identifications/{transactionId}/requestVideoChat\n  method: post\n  operationId: requestVideoChat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /{company}/identifications/{transactionId}\n  method: get\n  operationId: getIdentification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idnow/refs/heads/main/agentic-access/idnow-agentic-access.yml
summary_line: 5 operations · 4 acting
tags:
- Identity Verification
- KYC
- Identity Proofing
- AML
- eSign
---
