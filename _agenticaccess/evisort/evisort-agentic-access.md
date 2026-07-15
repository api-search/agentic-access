---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 2
api_specs:
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Documents API
  slug: documents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Field and Metadata Extraction API
  slug: field-extraction
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Workflow API
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
- filename: evisort-openapi.yml
  format: yaml
  label: Evisort Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/openapi/evisort-openapi.yml
consequence_counts:
  read: 2
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Evisort Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Evisort exposes 5 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Evisort
provider_slug: evisort
slug: evisort-agentic-access
source_filename: evisort-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/evisort-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 3\n    connected: 2\n  by_consequence:\n    write: 3\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: post\n  operationId: searchDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{evisortId}/content\n  method: get\n  operationId: getDocumentContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{evisortId}/fields\n  method: get\n  operationId: getDocumentFields\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evisort/refs/heads/main/agentic-access/evisort-agentic-access.yml
summary_line: 5 operations · 3 acting
tags:
- Contract Lifecycle Management
- CLM
- Contract Intelligence
- Document AI
- Legal Tech
---
