---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: element5-openapi-original.json
  format: json
  label: Element5 API
  slug: element5-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element5/refs/heads/main/openapi/element5-openapi-original.json
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Element5 Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Element5 exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Element5
provider_slug: element5
slug: element5-agentic-access
source_filename: element5-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/element5-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 4\n    acting: 4\n  by_consequence:\n    read: 4\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /store/v1/file-object/{object-id}\n  method: get\n  operationId: getFileObject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /store/v1/file-object\n  method: put\n  operationId: uploadFileObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wf/v2/workflows/submit-authorization\n  method: post\n  operationId: submitAuthorizationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wf/v2/workflows/submit-authorization/{task-id}\n  method: get\n  operationId: getSubmitAuthorizationRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wf/v2/workflows/submit-eligibility\n  method: post\n  operationId: submitEligibilityRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wf/v2/workflows/submit-eligibility/{task-id}\n  method: get\n  operationId: getSubmitEligibilityRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /wf/v2/workflows/process-x12-eligibility-transaction\n  method: post\n  operationId: processX12EligibilityTransactionRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wf/v2/workflows/process-x12-eligibility-transaction/{task-id}\n  method: get\n  operationId: getProcessX12EligibilityTransactionRequestStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/element5/refs/heads/main/agentic-access/element5-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Post-Acute Care
- Workflow Automation
- Eligibility Verification
- Prior Authorization
- Claims Processing
- Webhooks
- Artificial Intelligence
---
