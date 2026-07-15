---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Envelopes API
  slug: signeasy-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Originals API
  slug: signeasy-originals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Templates API
  slug: signeasy-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Embedded Signing API
  slug: signeasy-embedded-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Webhooks API
  slug: signeasy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
- filename: signeasy-openapi.yml
  format: yaml
  label: Signeasy Users API
  slug: signeasy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/openapi/signeasy-openapi.yml
consequence_counts:
  physical: 2
  read: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Signeasy Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rs/embedded/url/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rs/envelope/
operation_count: 12
overview: 'Signeasy exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 7 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Signeasy
provider_slug: signeasy
slug: signeasy-agentic-access
source_filename: signeasy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/signeasy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 9\n    connected: 3\n  by_consequence:\n    physical: 2\n    read: 3\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /rs/envelope/\n  method: post\n  operationId: createEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rs/envelope/{pending_file_id}\n  method: get\n\
  \  operationId: getEnvelope\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rs/envelope/{pending_file_id}/cancel\n  method: post\n  operationId: cancelEnvelope\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rs/{rs_id}/cancel\n  method: post\n  operationId: cancelSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rs/envelope/signed/{signed_id}/{source_id}/download\n  method: get\n  operationId: downloadSignedFile\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /original/\n  method: post\n  operationId: uploadOriginal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/{template_id}\n  method: put\n  operationId: updateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/{template_id}/embed\n  method: post\n  operationId: fetchEmbeddedTemplateCreateUrl\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rs/embedded/url/\n  method: post\n  operationId: fetchEmbeddedSendingUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rs/embedded/{pending_file_id}/cancel/\n  method: post\n  operationId: cancelEmbeddedSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /rs/embedded/signing_url/\n  method: post\n  operationId: fetchEmbeddedSigningUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me/\n  method: get\n  operationId: fetchUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signeasy/refs/heads/main/agentic-access/signeasy-agentic-access.yml
summary_line: 12 operations · 9 acting
tags:
- eSignature
- Electronic Signature
- Documents
- Contract Management
- Embedded Signing
- Templates
- Webhooks
---
