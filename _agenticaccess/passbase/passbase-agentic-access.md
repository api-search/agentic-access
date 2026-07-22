---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: passbase-verification-openapi.yml
  format: yaml
  label: Passbase Verifications API
  slug: passbase-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passbase/refs/heads/main/openapi/passbase-verification-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Passbase Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Passbase exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Passbase
provider_slug: passbase
slug: passbase-agentic-access
source_filename: passbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/passbase-verification-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /identities\n  method: get\n  operationId: listIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identities/{id}\n  method: get\n  operationId: getIdentityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/{id}/resources\n  method: get\n  operationId:\
  \ listIdentityResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/{id}/resources/{resource_id}\n  method: get\n  operationId: getIdentityResourceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity/{id}/resources/{resource_id}/resource_files/{resource_file_id}\n  method: get\n  operationId: getIdentityResourceFileById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settings\n  method: get\n  operationId: getSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passbase/refs/heads/main/agentic-access/passbase-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Security
- Identity Verification
- KYC
- Biometrics
- Authentication
- Identity
- Compliance
---
