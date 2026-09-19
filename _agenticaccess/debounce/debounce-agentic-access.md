---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: debounce-account-management-api-openapi.yml
  format: yaml
  label: DeBounce Account Management API
  slug: debounce-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-account-management-api-openapi.yml
- filename: debounce-debounce-disposable-email-detector-api-api-openapi.yml
  format: yaml
  label: DeBounce Disposable Email Detector API
  slug: debounce-debounce-disposable-email-detector-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-debounce-disposable-email-detector-api-api-openapi.yml
- filename: debounce-debounce-email-validation-api-api-openapi.yml
  format: yaml
  label: DeBounce Email Validation API
  slug: debounce-debounce-email-validation-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-debounce-email-validation-api-api-openapi.yml
- filename: debounce-reverse-api-openapi.yml
  format: yaml
  label: DeBounce Reverse API
  slug: debounce-reverse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-reverse-api-openapi.yml
- filename: debounce-status-api-openapi.yml
  format: yaml
  label: DeBounce Status API
  slug: debounce-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-status-api-openapi.yml
- filename: debounce-upload-api-openapi.yml
  format: yaml
  label: DeBounce Upload API
  slug: debounce-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-upload-api-openapi.yml
- filename: debounce-usage-api-openapi.yml
  format: yaml
  label: DeBounce Usage API
  slug: debounce-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-usage-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Debounce Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'DeBounce exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DeBounce
provider_slug: debounce
slug: debounce-agentic-access
source_filename: debounce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/debounce-account-api-openapi.yml, openapi/debounce-bulk-api-openapi.yml, openapi/debounce-data-api-openapi.yml,\n  openapi/debounce-disposable-api-openapi.yml, openapi/debounce-validation-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/balance/\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage/\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/upload/\n  method: get\n  operationId: uploadBulkList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status/\n  method: get\n  operationId: checkBulkStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reverse/\n  method: get\n  operationId: reverseEmailLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: checkDisposableEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/\n  method: get\n  operationId: validateEmail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/agentic-access/debounce-agentic-access.yml
summary_line: 7 operations
tags:
- Email Validation
- Email Verification
- Deliverability
- Disposable Email Detection
- MX Records
- Bulk Email Validation
- Data Enrichment
- Syntax Validation
- Reverse Email Lookup
- Logo API
---
