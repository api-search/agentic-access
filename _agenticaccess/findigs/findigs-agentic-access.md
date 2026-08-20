---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 6
api_specs:
- filename: findigs-client-api-openapi.yml
  format: yaml
  label: Findigs Client API
  slug: findigs-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/openapi/findigs-client-api-openapi.yml
consequence_counts:
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Findigs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Findigs exposes 8 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Findigs
provider_slug: findigs
slug: findigs-agentic-access
source_filename: findigs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: openapi/findigs-client-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 6\n    acting: 2\n  by_consequence:\n    read: 6\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /listings/\n  method: get\n  operationId: get_listings_listings__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/\n  method: post\n  operationId: post_listing_listings__post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/{listing_id}\n  method: get\n  operationId: get_listing_listings__listing_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/{listing_id}\n  method: patch\n  operationId: patch_listing_listings__listing_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/\n  method: get\n  operationId: get_applications_applications__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}\n\
  \  method: get\n  operationId: get_application_applications__application_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/\n  method: get\n  operationId: get_groups_groups__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{group_id}\n  method: get\n  operationId: get_group_groups__group_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/agentic-access/findigs-agentic-access.yml
summary_line: 8 operations · 2 acting
tags:
- rental-screening
- Tenant Screening
- resident-screening
- rental-application
- Underwriting
- Decisioning
- Identity Verification
- Income Verification
- Credit Check
- Background Check
- Fraud Detection
- Property Management
- Real-Estate
- PropTech
- FCRA
- Fair Housing
- Webhook
---
