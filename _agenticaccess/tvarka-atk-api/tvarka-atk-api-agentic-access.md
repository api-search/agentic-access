---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 7
api_specs:
- filename: tvarka-atk-api-auth-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Auth API
  slug: tvarka-atk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-auth-api-openapi.yml
- filename: tvarka-atk-api-erasure-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Erasure API
  slug: tvarka-atk-api-erasure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-erasure-api-openapi.yml
- filename: tvarka-atk-api-ltv-api-openapi.yml
  format: yaml
  label: Tvarka ATK API LTV API
  slug: tvarka-atk-api-ltv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-ltv-api-openapi.yml
- filename: tvarka-atk-api-pairing-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Pairing API
  slug: tvarka-atk-api-pairing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-pairing-api-openapi.yml
- filename: tvarka-atk-api-sign-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Sign API
  slug: tvarka-atk-api-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-sign-api-openapi.yml
- filename: tvarka-atk-api-tvarka-atk-api-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Tvarka ATK API API
  slug: tvarka-atk-api-tvarka-atk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-tvarka-atk-api-api-openapi.yml
- filename: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Tvarka ATK QES Signing API (paid Tier Addendum) API
  slug: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api-openapi.yml
- filename: tvarka-atk-api-validation-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Validation API
  slug: tvarka-atk-api-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-validation-api-openapi.yml
- filename: tvarka-atk-api-well-known-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Well Known API
  slug: tvarka-atk-api-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-well-known-api-openapi.yml
consequence_counts:
  read: 7
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tvarka Atk Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 22
overview: 'Tvarka ATK API exposes 22 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tvarka ATK API
provider_slug: tvarka-atk-api
slug: tvarka-atk-api-agentic-access
source_filename: tvarka-atk-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/tvarka-atk-api-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 15\n    connected: 7\n  by_consequence:\n    write: 15\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/requests\n  method: post\n  operationId: createAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/{requestId}/certificate\n  method: post\n  operationId: submitAuthCertificate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/{requestId}/complete\n  method: post\n  operationId: completeAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/{requestId}\n  method: get\n  operationId: getAuthRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/{requestId}/cancel\n  method: post\n  operationId: cancelAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/{requestId}/delete\n  method: post\n  operationId: deleteAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /erasure\n  method: post\n  operationId: bulkErasure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/{requestId}/pairing\n  method: get\n  operationId: getAuthPairing\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pairing/claim\n  method: post\n  operationId: claimPairing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/atk-jwks.json\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sign/requests\n  method: post\n  operationId: createSignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /sign/{requestId}/certificate\n  method: post\n  operationId: submitSignCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sign/{requestId}/complete\n  method: post\n  operationId: completeSign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sign/{requestId}\n  method: get\n  operationId: getSignRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sign/{requestId}/document\n\
  \  method: get\n  operationId: downloadSignedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sign/{requestId}/cancel\n  method: post\n  operationId: cancelSignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sign/{requestId}/delete\n  method: post\n  operationId: deleteSignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sign/{requestId}/pairing\n  method: get\n  operationId: getSignPairing\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /validation\n  method: post\n  operationId: validateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /timestamp\n  method: post\n  operationId: timestampDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /archive\n  method: post\n  operationId: archiveDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/{requestId}/document\n  method: get\n  operationId: downloadServiceDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\nnote: 'Deduplicated to the canonical complete contract: the provider also publishes specialist auth.yaml\n  and sign.yaml views that repeat the same operations, so the raw derivation counted 45.'\nx-review:\n- HEURISTIC OUTPUT - not a Tvarka claim. Review before binding.\n- createSignRequest and completeSign produce a QUALIFIED ELECTRONIC SIGNATURE with legal effect under\n  eIDAS; treat them as human-in-the-loop required, above the heuristic default.\n- completeAuth produces a verified national eID identity; it should not run without a present card holder.\n- deleteAuthRequest,\
  \ deleteSignRequest and bulkErasure are irreversible GDPR erasures; treat as human-in-the-loop\n  required.\n- validateDocument, timestampDocument and archiveDocument carry a required Idempotency-Key, so an agent\n  retry there is genuinely safe.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/agentic-access/tvarka-atk-api-agentic-access.yml
summary_line: 22 operations · 15 acting
tags:
- Authentication
- Digital Signature
- eIDAS
- QES
- Lithuania
- OpenAPI
- eID
- Smart-ID
- Mobile-ID
- NFC
- Timestamping
- LTV
- Webhooks
- Identity
- Trust Services
- GDPR
---
