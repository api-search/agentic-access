---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: easyemailverification-com-account-api-openapi.yml
  format: yaml
  label: Easy Email Verification Account API
  slug: easyemailverification-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-account-api-openapi.yml
- filename: easyemailverification-com-bulk-verification-api-openapi.yml
  format: yaml
  label: Easy Email Verification Bulk Verification API
  slug: easyemailverification-com-bulk-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-bulk-verification-api-openapi.yml
- filename: easyemailverification-com-single-verification-api-openapi.yml
  format: yaml
  label: Easy Email Verification Single Verification API
  slug: easyemailverification-com-single-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easyemailverification-com/openapi/easyemailverification-com-single-verification-api-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Easyemailverification Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Easy Email Verification exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Easy Email Verification
provider_slug: easyemailverification-com
slug: easyemailverification-com-agentic-access
source_filename: easyemailverification-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/easyemailverification-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 5\n    acting: 3\n  by_consequence:\n    read: 5\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /verify\n  method: get\n  operationId: verify\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: post\n  operationId: verifyBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk/upload\n  method: post\n  operationId: uploadBulkFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk/status\n  method: get\n  operationId: listBulkJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/status/{id}\n  method: get\n  operationId: getBulkJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/download/{id}\n  method: get\n  operationId: downloadBulkResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk/{id}\n  method: delete\n  operationId: deleteBulkJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/easyemailverification-com/agentic-access/easyemailverification-com-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Email Verification
- Software-as-a-Service
- Data Validation
- Marketing
---
