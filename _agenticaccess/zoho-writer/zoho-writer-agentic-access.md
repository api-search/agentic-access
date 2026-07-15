---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 5
api_specs:
- filename: zoho-writer-openapi.json
  format: json
  label: Zoho Writer API
  slug: zoho-writer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-writer/refs/heads/main/openapi/zoho-writer-openapi.json
consequence_counts:
  read: 5
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zoho Writer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Zoho Writer exposes 12 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zoho Writer
provider_slug: zoho-writer
slug: zoho-writer-agentic-access
source_filename: zoho-writer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/zoho-writer-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 5\n    acting: 7\n  by_consequence:\n    read: 5\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - WorkDrive.files.ALL\n    - WorkDrive.organization.ALL\n    - WorkDrive.workspace.ALL\n    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents\n  method: post\n  operationId: createDocument\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - WorkDrive.files.ALL\n    - WorkDrive.organization.ALL\n    - WorkDrive.workspace.ALL\n    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - WorkDrive.files.ALL\n    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n- path: /documents/{document_id}/metrics\n  method: get\n  operationId: getDocumentMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - WorkDrive.files.ALL\n\
  \    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n- path: /download/{document_id}\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - WorkDrive.files.ALL\n    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /documents/{document_id}/merge\n  method: post\n  operationId: mergeDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WorkDrive.files.ALL\n    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n    - ZohoWriter.merge.ALL\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/merge/sign\n  method: post\n  operationId: mergeAndSign\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - WorkDrive.files.ALL\n    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n    - ZohoWriter.merge.ALL\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}/merge/execute\n  method: post\n  operationId: mergeAndInvoke\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoWriter.documentEditor.ALL\n    - ZohoWriter.merge.ALL\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/v2/{document_id}/merge/store\n  method: post\n  operationId: mergeAndStoreV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    scope:\n    - WorkDrive.files.ALL\n    - WorkDrive.organization.ALL\n    - ZohoWriter.documentEditor.ALL\n    - ZohoWriter.merge.ALL\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/pdf/combine\n  method: post\n  operationId: combinePdfs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - WorkDrive.organization.ALL\n    - ZohoWriter.documentEditor.ALL\n    - ZohoWriter.merge.ALL\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/pdf/combine/job/{job_id}\n  method: get\n  operationId: getCombineJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n    scope:\n    - WorkDrive.files.ALL\n    - ZohoPC.files.ALL\n    - ZohoWriter.documentEditor.ALL\n- path: /templates/{template_id}/bulkmerge/sign\n  method: post\n  operationId: bulkMergeAndSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - ZohoWriter.documentEditor.ALL\n    - ZohoWriter.merge.ALL\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-writer/refs/heads/main/agentic-access/zoho-writer-agentic-access.yml
summary_line: 12 operations · 7 acting
tags:
- Documents
- Word Processor
- Mail Merge
- Document Generation
- Electronic Signatures
- Zoho
- Office Suite
- Automation
---
