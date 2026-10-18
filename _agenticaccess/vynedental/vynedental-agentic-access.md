---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 5
api_specs:
- filename: vynedental-eligibility-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility and Benefits API (Onederful)
  slug: eligibility-and-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-api-openapi.yml
- filename: vynedental-async-api-openapi.yml
  format: yaml
  label: Vyne Dental Async API
  slug: vynedental-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-async-api-openapi.yml
- filename: vynedental-edi-api-openapi.yml
  format: yaml
  label: Vyne Dental EDI API
  slug: vynedental-edi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-edi-api-openapi.yml
- filename: vynedental-eligibility-response-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility Response API
  slug: vynedental-eligibility-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-response-api-openapi.yml
- filename: vynedental-eligibility-status-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility Status API
  slug: vynedental-eligibility-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-status-api-openapi.yml
- filename: vynedental-enhanced-eligibility-api-openapi.yml
  format: yaml
  label: Vyne Dental Enhanced Eligibility API
  slug: vynedental-enhanced-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-enhanced-eligibility-api-openapi.yml
- filename: vynedental-oauth2-api-openapi.yml
  format: yaml
  label: Vyne Dental Oauth2 API
  slug: vynedental-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-oauth2-api-openapi.yml
- filename: vynedental-well-known-api-openapi.yml
  format: yaml
  label: Vyne Dental .well Known API
  slug: vynedental-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-well-known-api-openapi.yml
consequence_counts:
  read: 5
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vynedental Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Vyne Dental exposes 17 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vyne Dental
provider_slug: vynedental
slug: vynedental-agentic-access
source_filename: vynedental-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/vynedental-eligibility-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    acting: 12\n    connected: 5\n  by_consequence:\n    write: 12\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /async/eligibility\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /async/eligibility/sequenced-search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /async/edi/eligibility\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /async/edi/eligibility/sequenced-search\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /async/enhanced-eligibility\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /async/enhanced-eligibility/targeted\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eligibility-response/{onederfulId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eligibility-response/{onederfulId}/html\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eligibility-response/{onederfulId}/edi\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eligibility\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enhanced-eligibility\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /enhanced-eligibility/targeted\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eligibility-status/{onederfulId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /edi/eligibility\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token/invalidate\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/jwks.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/agentic-access/vynedental-agentic-access.yml
summary_line: 17 operations · 12 acting
tags:
- Company
- Dental
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- Payments
---
