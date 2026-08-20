---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 6
api_specs:
- filename: brellium-audits-api-openapi.yml
  format: yaml
  label: Brellium Audits API
  slug: brellium-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-audits-api-openapi.yml
- filename: brellium-auth-api-openapi.yml
  format: yaml
  label: Brellium Auth API
  slug: brellium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-auth-api-openapi.yml
- filename: brellium-coding-api-openapi.yml
  format: yaml
  label: Brellium Coding API
  slug: brellium-coding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-coding-api-openapi.yml
- filename: brellium-documents-api-openapi.yml
  format: yaml
  label: Brellium Documents API
  slug: brellium-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-documents-api-openapi.yml
- filename: brellium-documents-multiple-api-openapi.yml
  format: yaml
  label: Brellium Documents Multiple API
  slug: brellium-documents-multiple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-documents-multiple-api-openapi.yml
- filename: brellium-link-providers-api-openapi.yml
  format: yaml
  label: Brellium Link Providers API
  slug: brellium-link-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-link-providers-api-openapi.yml
- filename: brellium-question-sets-api-openapi.yml
  format: yaml
  label: Brellium Question Sets API
  slug: brellium-question-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-question-sets-api-openapi.yml
- filename: brellium-update-audits-flags-api-openapi.yml
  format: yaml
  label: Brellium Update Audits Flags API
  slug: brellium-update-audits-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-update-audits-flags-api-openapi.yml
- filename: brellium-users-api-openapi.yml
  format: yaml
  label: Brellium Users API
  slug: brellium-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-users-api-openapi.yml
consequence_counts:
  read: 6
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brellium Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Brellium exposes 17 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brellium
provider_slug: brellium
slug: brellium-agentic-access
source_filename: brellium-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/brellium-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 11\n    connected: 6\n  by_consequence:\n    write: 11\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /auth\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/upload-url\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents-multiple\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{document_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /audits\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /audits/{audit_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /coding\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /coding/{coding_eval_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /users\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{user_id}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /users/{user_id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /question-sets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-audits-flags\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /link-providers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/agentic-access/brellium-agentic-access.yml
summary_line: 17 operations · 11 acting
tags:
- Company
- Healthcare
- Clinical Compliance
- Clinical Documentation
- Medical Coding
- Audit
- Behavioral Health
- Digital Health
---
