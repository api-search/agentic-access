---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Contracts API
  slug: sirion-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Contract Requests API
  slug: sirion-contract-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Metadata & Clauses API
  slug: sirion-metadata-clauses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Obligations API
  slug: sirion-obligations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Suppliers & Counterparties API
  slug: sirion-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
- filename: sirion-openapi.yml
  format: yaml
  label: Sirion Integrations & Webhooks API
  slug: sirion-integrations-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/openapi/sirion-openapi.yml
consequence_counts:
  read: 8
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sirion Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Sirion exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sirion
provider_slug: sirion
slug: sirion-agentic-access
source_filename: sirion-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sirion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /contracts\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: post\n  operationId: createContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contractId}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contractId}\n  method: patch\n  operationId: updateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract-requests\n  method: get\n  operationId: listContractRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract-requests\n  method: post\n  operationId: createContractRequest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contractId}/metadata\n  method: get\n  operationId: getContractMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contractId}/metadata\n  method: patch\n  operationId: updateContractMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contractId}/clauses\n  method: get\n  operationId: listContractClauses\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /obligations\n  method: get\n  operationId: listObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /obligations/{obligationId}\n  method: patch\n  operationId: updateObligation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /suppliers\n  method: get\n  operationId: listSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppliers\n  method: post\n  operationId: createSupplier\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirion/refs/heads/main/agentic-access/sirion-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- AI
- Enterprise
- Legal
- Agreements
- Supplier Management
- Obligations
---
