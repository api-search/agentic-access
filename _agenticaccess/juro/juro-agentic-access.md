---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 7
api_specs:
- filename: juro-openapi.yml
  format: yaml
  label: Juro Contracts API
  slug: juro-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
- filename: juro-openapi.yml
  format: yaml
  label: Juro Templates API
  slug: juro-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
- filename: juro-openapi.yml
  format: yaml
  label: Juro Signatures API
  slug: juro-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
- filename: juro-openapi.yml
  format: yaml
  label: Juro Webhooks API
  slug: juro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/openapi/juro-openapi.yml
consequence_counts:
  physical: 2
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Juro Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contracts/{contract_id}/signing-request/{signing_side_uid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /contracts/{contract_id}/signing-request/{signing_side_uid}/signatures/{signature_uid}
operation_count: 16
overview: 'Juro exposes 16 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 7 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Juro
provider_slug: juro
slug: juro-agentic-access
source_filename: juro-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/juro-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 7\n    acting: 9\n  by_consequence:\n    read: 7\n    write: 7\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{template_id}\n  method: get\n\
  \  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: post\n  operationId: createContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/upload\n  method: post\n  operationId: uploadContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}\n  method: patch\n  operationId: updateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}\n  method: delete\n  operationId: deleteContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /contracts/{contract_id}/pdf/binary\n  method: get\n  operationId: getContractPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contract_id}/sign\n  method: post\n  operationId: signContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/signing-request/{signing_side_uid}\n  method: post\n  operationId: sendSigningRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contract_id}/signing-request/{signing_side_uid}/signatures/{signature_uid}\n  method: post\n  operationId: sendSigningRequestToSignatory\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juro/refs/heads/main/agentic-access/juro-agentic-access.yml
summary_line: 16 operations · 9 acting
tags:
- Contract Management
- CLM
- Contract Lifecycle
- Contract Automation
- Legal
- LegalTech
- E-Signature
- Contracts
---
