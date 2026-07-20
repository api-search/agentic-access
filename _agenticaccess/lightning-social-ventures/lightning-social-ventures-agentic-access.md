---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: lightning-social-ventures-lightning-reach-openapi.json
  format: json
  label: Lightning Reach API
  slug: lightning-reach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightning-social-ventures/refs/heads/main/openapi/lightning-social-ventures-lightning-reach-openapi.json
consequence_counts:
  read: 6
  safety-critical: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Lightning Social Ventures Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/applications
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/applications/{id}/referral
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/applications/{id}/status
operation_count: 9
overview: 'Lightning Social Ventures exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lightning Social Ventures
provider_slug: lightning-social-ventures
slug: lightning-social-ventures-agentic-access
source_filename: lightning-social-ventures-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/lightning-social-ventures-lightning-reach-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /v1/applications\n  method: get\n  operationId: PublicGrantApplicationsController_findAll_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications\n  method: post\n  operationId: PublicGrantApplicationsController_submitApplication_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/applications/{id}\n  method: get\n  operationId: PublicGrantApplicationsController_findById_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{id}/assets\n  method: get\n  operationId: PublicGrantApplicationsController_getFiles_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applications/{id}/status\n  method: put\n  operationId: PublicGrantApplicationsController_updateStatusById_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/applications/{id}/referral\n  method: post\n  operationId: PublicGrantApplicationsController_submitApplicationReferral_v1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/support-schemes\n  method: get\n  operationId: PublicGrantsController_findAll_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: PublicWebhooksController_findAll_v1\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks/keys/{id}/public\n  method: get\n  operationId: PublicWebhooksController_getPublicKey_v1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightning-social-ventures/refs/heads/main/agentic-access/lightning-social-ventures-agentic-access.yml
summary_line: 9 operations · 3 acting · 3 human-in-the-loop
tags:
- Company
- Financial Inclusion
- Grants
- Social Impact
- Nonprofit
- Housing
- Government
- Welfare Benefits
- United Kingdom
---
