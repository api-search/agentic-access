---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: hhaexchange-fhir-openapi.yml
  format: yaml
  label: HHAeXchange EVV API
  slug: hhaexchange-evv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhaexchange/refs/heads/main/openapi/hhaexchange-fhir-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hhaexchange Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'HHAeXchange exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HHAeXchange
provider_slug: hhaexchange
slug: hhaexchange-agentic-access
source_filename: hhaexchange-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hhaexchange-fhir-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/fhir-onboarding/client\n  method: post\n  operationId: create_client_v1_fhir_onboarding_client_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full_access\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fhir-onboarding/client/migrate\n\
  \  method: post\n  operationId: migrate_client_v1_fhir_onboarding_client_migrate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full_access\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/fhir-onboarding/client/{client_id}\n  method: get\n  operationId: get_client_v1_fhir_onboarding_client__client_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full_access\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fhir-onboarding/client/{client_id}\n  method: patch\n  operationId: update_client_v1_fhir_onboarding_client__client_id__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - full_access\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/internal/provider\n  method: get\n  operationId: get_provider_v1_internal_provider_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full_access\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/internal/generic-references\n  method: get\n  operationId: get_generic_references_v1_internal_generic_references_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full_access\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/internal/payer\n  method: get\n  operationId: get_payer_v1_internal_payer_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full_access\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/rate-limits/config\n  method: get\n  operationId: get_rate_limit_config_v1_rate_limits_config_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - full_access\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hhaexchange/refs/heads/main/agentic-access/hhaexchange-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Homecare
- EVV
- Electronic Visit Verification
- Medicaid
- Scheduling
- Caregiver
- Healthcare
---
