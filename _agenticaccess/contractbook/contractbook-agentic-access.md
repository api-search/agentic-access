---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 7
api_specs:
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Documents API
  slug: contractbook-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Templates API
  slug: contractbook-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Document Sharing API
  slug: contractbook-document-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Automations API
  slug: contractbook-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Spaces API
  slug: contractbook-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
- filename: contractbook-openapi.json
  format: json
  label: Contractbook Attachments API
  slug: contractbook-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/openapi/contractbook-openapi.json
consequence_counts:
  physical: 1
  read: 7
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Contractbook Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /documents/{id}/send
operation_count: 16
overview: 'Contractbook exposes 16 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Contractbook
provider_slug: contractbook
slug: contractbook-agentic-access
source_filename: contractbook-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/contractbook-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 7\n    acting: 9\n  by_consequence:\n    read: 7\n    write: 8\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /automations\n  method: get\n  operationId: list_automations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automations/{id}/run\n  method: post\n  operationId: run_automation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: get\n  operationId: list_documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: delete\n  operationId: delete_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}\n  method: get\n  operationId: get_document_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}\n  method: patch\n  operationId: update_document\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/pdf\n  method: get\n  operationId: get_pdf_document_by_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{id}/send\n  method: post\n  operationId: send_document\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/share\n  method: delete\n  operationId: unshare_document\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}/share\n  method: post\n  operationId: share_document\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{id}\n  method: post\n  operationId: create_child_space\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /spaces/{id}/tree\n  method: get\n  operationId: get_space_tree\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates\n  method: get\n  operationId: get_templates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{id}\n  method: get\n  operationId: get_template\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /templates/{id}/create_document\n  method: post\n  operationId: create_document_from_template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /upload\n  method: post\n  operationId:\
  \ create_attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contractbook/refs/heads/main/agentic-access/contractbook-agentic-access.yml
summary_line: 16 operations · 9 acting
tags:
- Contract Management
- CLM
- Contract Lifecycle
- Legal
- eSignature
- Contracts
- Document Automation
- LegalTech
---
