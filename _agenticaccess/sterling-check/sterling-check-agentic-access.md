---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 7
api_specs:
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Screenings API
  slug: sterling-check-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Candidates API
  slug: sterling-check-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Packages API
  slug: sterling-check-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Reports API
  slug: sterling-check-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Invites API
  slug: sterling-check-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Webhooks API
  slug: sterling-check-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
consequence_counts:
  physical: 1
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sterling Check Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /screenings/{screeningId}/invite
operation_count: 15
overview: 'Sterling exposes 15 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 7 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sterling
provider_slug: sterling-check
slug: sterling-check-agentic-access
source_filename: sterling-check-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sterling-check-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 8\n    connected: 7\n  by_consequence:\n    write: 7\n    read: 7\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /packages\n  method: get\n  operationId: listPackages\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{packageId}\n  method: get\n  operationId: getPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates\n  method: post\n  operationId: createCandidate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /candidates/{candidateId}\n  method: get\n  operationId: getCandidate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /candidates/{candidateId}\n  method: patch\n  operationId: updateCandidate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screenings\n  method: get\n  operationId: listScreenings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screenings\n  method: post\n  operationId: createScreening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screenings/{screeningId}\n  method: get\n  operationId: getScreening\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /screenings/{screeningId}/cancel\n  method: post\n  operationId: cancelScreening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screenings/{screeningId}/invite\n  method: post\n  operationId: resendInvite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screenings/{screeningId}/report\n  method: get\n  operationId: getScreeningReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/agentic-access/sterling-check-agentic-access.yml
summary_line: 15 operations · 8 acting
tags:
- Background Screening
- Identity Verification
- Background Check
- HR Tech
- Compliance
- Gated API
---
