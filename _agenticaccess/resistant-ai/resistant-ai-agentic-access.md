---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 11
api_specs:
- filename: resistant-ai-documents-openapi.json
  format: json
  label: Resistant Documents API
  slug: resistant-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-documents-openapi.json
- filename: resistant-ai-tenant-management-openapi.json
  format: json
  label: Resistant Documents Tenant Management API
  slug: resistant-documents-tenant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-tenant-management-openapi.json
consequence_counts:
  read: 11
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Resistant Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Resistant AI exposes 19 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Resistant AI
provider_slug: resistant-ai
slug: resistant-ai-agentic-access
source_filename: resistant-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/resistant-ai-documents-openapi.json, openapi/resistant-ai-tenant-management-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 8\n    connected: 11\n  by_consequence:\n    write: 8\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/submission\n  method: post\n  operationId: createSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submissions.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/submission/{submission_id}/characteristics\n\
  \  method: put\n  operationId: putSubmissionCharacteristics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submissions.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/submission/{submission_id}/fraud\n  method: get\n  operationId: getFraud\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - submissions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/submission/{submission_id}/content\n  method: get\n  operationId: getContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - submissions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/submission/{submission_id}/quality\n  method: get\n  operationId: getQuality\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - submissions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/submission/{submission_id}/decision\n  method: get\n  operationId: getDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - submissions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/submission/{submission_id}/classification\n  method: get\n  operationId: getClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - submissions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/submission/{submission_id}/report\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - submissions.read\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /v2/submission/{submission_id}\n  method: delete\n  operationId: deleteSubmission\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submissions.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/submission/{submission_id}/feedback\n  method: put\n  operationId: putFeedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - submissions.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/submission/{submission_id}/feedback\n  method: get\n  operationId: getFeedback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    scope:\n    - submissions.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants\n  method: post\n  operationId: createTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenants.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants\n  method: get\n  operationId: getTenants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenants.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}\n  method: get\n  operationId: getTenant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenants.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}\n  method: delete\n\
  \  operationId: deleteTenant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenants.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/applications\n  method: get\n  operationId: getTenantApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenants.applications.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/applications\n  method: post\n  operationId: createTenantApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenants.applications.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /tenants/{tenant_id}/applications/{application_id}\n  method: get\n  operationId: getTenantApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - tenants.applications.read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenants/{tenant_id}/applications/{application_id}\n  method: delete\n  operationId: deleteTenantApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - tenants.applications.write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/agentic-access/resistant-ai-agentic-access.yml
summary_line: 19 operations · 8 acting
tags:
- Company
- Ai
- Fraud Detection
- Financial Crime
- Document Verification
- Document Forensics
- AML
- Identity Verification
- Fintech
- Machine Learning
---
