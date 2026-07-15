---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 10
api_specs:
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Transcriptions API
  slug: happyscribe-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Orders API
  slug: happyscribe-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Exports API
  slug: happyscribe-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Organizations API
  slug: happyscribe-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Organization Memberships API
  slug: happyscribe-organization-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Uploads API
  slug: happyscribe-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
- filename: happyscribe-openapi.yml
  format: yaml
  label: Happy Scribe Glossaries and Style Guides API
  slug: happyscribe-glossaries-style-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/openapi/happyscribe-openapi.yml
consequence_counts:
  physical: 6
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Happyscribe Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/translation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/{id}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /organization_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /organization_memberships/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /organization_memberships/{id}
operation_count: 20
overview: 'Happy Scribe exposes 20 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 4 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Happy Scribe
provider_slug: happyscribe
slug: happyscribe-agentic-access
source_filename: happyscribe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/happyscribe-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 10\n    acting: 10\n  by_consequence:\n    read: 10\n    write: 4\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /transcriptions\n  method: get\n  operationId: listTranscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transcriptions\n  method: post\n  operationId: createTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transcriptions/{id}\n  method: get\n  operationId: getTranscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transcriptions/{id}\n  method: patch\n  operationId: updateTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transcriptions/{id}\n  method: delete\n  operationId: deleteTranscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /transcriptions/{id}/summary\n  method: get\n  operationId: getTranscriptionSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/translation\n  method: post\n  operationId: createTranslationOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{id}\n  method: get\n  operationId: getOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{id}/confirm\n  method: post\n  operationId: confirmOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exports\n  method: post\n  operationId: createExport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /exports/{id}\n  method: get\n  operationId: getExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organizations\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization_memberships\n  method: get\n  operationId: listOrganizationMemberships\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organization_memberships\n  method: post\n  operationId: createOrganizationMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization_memberships/{id}\n  method: patch\n  operationId: updateOrganizationMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organization_memberships/{id}\n  method: delete\n  operationId: deleteOrganizationMembership\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /uploads/new\n  method: get\n  operationId: newUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /glossaries\n  method: get\n  operationId: listGlossaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /style_guides\n  method: get\n  operationId: listStyleGuides\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyscribe/refs/heads/main/agentic-access/happyscribe-agentic-access.yml
summary_line: 20 operations · 10 acting
tags:
- Audio Transcription
- Transcription
- Speech-to-Text
- Subtitles
- Captions
- Translation
---
