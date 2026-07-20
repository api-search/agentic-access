---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 6
api_specs:
- filename: truora-openapi.yml
  format: yaml
  label: Truora Checks API
  slug: truora-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Validators API
  slug: truora-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Digital Identity API
  slug: truora-digital-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Account API
  slug: truora-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
consequence_counts:
  read: 6
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the modeled OpenAPI. A governance starting point for exposing this API to AI agents - review and bind audience per deployment. Because Truora operates on regulated personal identity data, write operations that create checks, validations, or identity processes carry a required human-in-the-loop, since they act on real people's PII and require explicit user authorization. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Truora Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Truora exposes 12 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 write.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Truora
provider_slug: truora
slug: truora-agentic-access
source_filename: truora-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/truora-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the modeled OpenAPI. A governance starting point for exposing this API to AI agents - review\n  and bind audience per deployment. Because Truora operates on regulated personal identity data,\n  write operations that create checks, validations, or identity processes carry a required\n  human-in-the-loop, since they act on real people's PII and require explicit user authorization.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 6\n    connected: 6\n  by_consequence:\n    write: 6\n    read: 6\n  human_in_the_loop_required: 4\noperations:\n- path: /v1/checks\n  method: post\n  operationId: createCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: required\n      triggers:\n      - pii\n      - high-value\n    audit: required\n- path: /v1/checks\n  method: get\n  operationId: listChecks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checks/{check_id}\n  method: get\n  operationId: getCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checks/{check_id}\n  method: delete\n  operationId: deleteCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checks/{check_id}/attachments\n  method: get\n  operationId: getCheckAttachments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/continuous-check\n  method: post\n  operationId: createContinuousCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - pii\n      - high-value\n    audit: required\n- path: /v1/validations\n  method: post\n  operationId: createValidation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - pii\n      - high-value\n    audit: required\n- path: /v1/validations/{validation_id}\n  method: get\n  operationId: getValidation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/processes/{process_id}\n  method: get\n  operationId: getProcess\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/processes/{process_id}/result\n  method: get\n  operationId: getProcessResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - credential-issuance\n      - high-value\n    audit: required\n- path: /v1/api-keys/{api_key_id}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/agentic-access/truora-agentic-access.yml
summary_line: 12 operations · 6 acting · 4 human-in-the-loop
tags:
- Identity Verification
- KYC
- Background Checks
- Fraud Prevention
- LatAm
- WhatsApp
---
