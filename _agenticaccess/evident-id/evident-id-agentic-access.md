---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 1
api_specs:
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Verification Requests API
  slug: evident-id-verification-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Attributes & Credentials API
  slug: evident-id-attributes-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Identity Assurance API
  slug: evident-id-identity-assurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Insurance & COI Verification API
  slug: evident-id-insurance-coi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Results API
  slug: evident-id-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Webhooks API
  slug: evident-id-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
consequence_counts:
  read: 1
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Evident Id Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'Evident exposes 3 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Evident
provider_slug: evident-id
slug: evident-id-agentic-access
source_filename: evident-id-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/evident-id-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 2\n    connected: 1\n  by_consequence:\n    write: 2\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /verify/requests\n  method: post\n  operationId: createVerificationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/requests/{requestId}\n  method: get\n  operationId: getVerificationRequest\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /requests\n  method: post\n  operationId: submitRequestData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/agentic-access/evident-id-agentic-access.yml
summary_line: 3 operations · 2 acting
tags:
- Identity Verification
- Credential Verification
- Background Check
- Insurance Verification
- COI
---
