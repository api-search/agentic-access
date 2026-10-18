---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: gstinapi-bulk-api-openapi.yml
  format: yaml
  label: GSTIN API Bulk API
  slug: gstinapi-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/openapi/gstinapi-bulk-api-openapi.yml
- filename: gstinapi-verification-api-openapi.yml
  format: yaml
  label: GSTIN API Verification API
  slug: gstinapi-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/openapi/gstinapi-verification-api-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gstinapi Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'GSTIN API exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GSTIN API
provider_slug: gstinapi
slug: gstinapi-agentic-access
source_filename: gstinapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/gstinapi-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/get-taxpayer-info/{gstin}\n  method: get\n  operationId: getTaxpayerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bulk/jobs\n  method: post\n  operationId: createBulkJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bulk/jobs\n  method: get\n  operationId: listBulkJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bulk/jobs/{job_id}\n  method: get\n  operationId: getBulkJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bulk/jobs/{job_id}\n  method: delete\n  operationId: cancelBulkJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/bulk/jobs/{job_id}/results\n  method: get\n  operationId: getBulkResults\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/agentic-access/gstinapi-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Company
- GST
- India
- Taxation
- API
---
