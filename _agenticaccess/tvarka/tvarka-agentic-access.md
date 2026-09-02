---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 13
api_specs:
- filename: tvarka-atk-api-auth-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Auth API
  slug: tvarka-atk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-auth-api-openapi.yml
- filename: tvarka-atk-api-erasure-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Erasure API
  slug: tvarka-atk-api-erasure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-erasure-api-openapi.yml
- filename: tvarka-atk-api-ltv-api-openapi.yml
  format: yaml
  label: Tvarka ATK API LTV API
  slug: tvarka-atk-api-ltv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-ltv-api-openapi.yml
- filename: tvarka-atk-api-pairing-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Pairing API
  slug: tvarka-atk-api-pairing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-pairing-api-openapi.yml
- filename: tvarka-atk-api-sign-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Sign API
  slug: tvarka-atk-api-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-sign-api-openapi.yml
- filename: auth.json
  format: json
  label: Tvarka ATK API Tvarka ATK API API
  slug: tvarka-atk-api-tvarka-atk-api-api
  spec_type: Postman
  url: https://atk.tvarka.pro/postman/auth.json
- filename: auth.json
  format: json
  label: Tvarka ATK API Tvarka ATK QES Signing API (paid Tier Addendum) API
  slug: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api
  spec_type: Postman
  url: https://atk.tvarka.pro/postman/auth.json
- filename: tvarka-atk-api-validation-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Validation API
  slug: tvarka-atk-api-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-validation-api-openapi.yml
- filename: tvarka-atk-api-well-known-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Well Known API
  slug: tvarka-atk-api-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-well-known-api-openapi.yml
- filename: tvarka-sign-api-openapi.yml
  format: yaml
  label: Tvarka Sign API
  slug: tvarka-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-sign-api-openapi.yml
consequence_counts:
  physical: 5
  read: 13
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 15
kind: agentic-access
layout: agentic-access
method: generated
name: Tvarka Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sign/requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sign/{requestId}/complete
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/batches
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/signings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/signings/{signingId}/signers
operation_count: 44
overview: 'Tvarka ATK API exposes 44 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read, 26 write, and 5 physical.


  15 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tvarka ATK API
provider_slug: tvarka
slug: tvarka-agentic-access
source_filename: tvarka-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: generated\nsource: openapi/tvarka-atk-api-auth-api-openapi.yml, openapi/tvarka-atk-api-erasure-api-openapi.yml, openapi/tvarka-atk-api-ltv-api-openapi.yml,\n  openapi/tvarka-atk-api-pairing-api-openapi.yml, openapi/tvarka-atk-api-sign-api-openapi.yml, openapi/tvarka-atk-api-validation-api-openapi.yml,\n  openapi/tvarka-atk-api-well-known-api-openapi.yml, openapi/tvarka-sign-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance\n  starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 44\n  by_action_class:\n    acting: 31\n    connected: 13\n  by_consequence:\n    write: 26\n    read: 13\n    physical: 5\n  human_in_the_loop_required: 15\noperations:\n- path: /auth/requests\n  method: post\n  operationId: createAuthRequest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Opens a national eID identity verification ceremony.\n- path: /auth/{requestId}/certificate\n  method: post\n  operationId: submitAuthCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/{requestId}/complete\n  method: post\n  operationId: completeAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Produces a verified national eID identity.\n- path: /auth/{requestId}\n  method: get\n  operationId: getAuthRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/{requestId}/cancel\n  method: post\n  operationId: cancelAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/{requestId}/delete\n  method: post\n  operationId: deleteAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Irreversible purge of a request and its personal data.\n- path: /erasure\n  method: post\n  operationId: bulkErasure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Irreversible tenant-wide purge of terminal request data.\n- path: /sign/{requestId}/delete\n  method: post\n  operationId: deleteSignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Irreversible purge of a request and its personal data.\n- path: /timestamp\n  method: post\n  operationId: timestampDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Billed trust-service call.\n- path: /archive\n  method: post\n  operationId: archiveDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Billed trust-service\
  \ call.\n- path: /services/{requestId}/document\n  method: get\n  operationId: downloadServiceDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/{requestId}/pairing\n  method: get\n  operationId: getAuthPairing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pairing/claim\n  method: post\n  operationId: claimPairing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sign/requests\n  method: post\n  operationId: createSignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Opens a QUALIFIED electronic signature ceremony with legal effect under eIDAS.\n- path: /sign/{requestId}/certificate\n  method: post\n  operationId: submitSignCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sign/{requestId}/complete\n  method: post\n  operationId: completeSign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Assembles the qualified signature. Irreversible once made.\n- path: /sign/{requestId}\n  method: get\n  operationId: getSignRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sign/{requestId}/document\n  method: get\n  operationId: downloadSignedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sign/{requestId}/cancel\n  method: post\n  operationId: cancelSignRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sign/{requestId}/pairing\n\
  \  method: get\n  operationId: getSignPairing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pairing/claim\n  method: post\n  operationId: claimPairing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /validation\n  method: post\n  operationId: validateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Billed trust-service call.\n- path: /.well-known/atk-jwks.json\n\
  \  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signings\n  method: get\n  operationId: listSignings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signings\n  method: post\n  operationId: createSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Opens a real, billed qualified signing ceremony and invites real people.\n- path: /v1/signings/{signingId}\n  method: get\n  operationId: getSigning\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signings/{signingId}\n  method: patch\n  operationId: updateSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signings/{signingId}\n  method: delete\n  operationId: eraseSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Cancels then irreversibly purges a signing.\n- path: /v1/batches\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Opens one billed signing per document for a set of parties.\n- path: /v1/batches/{batchId}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signings/{signingId}/archive\n  method: post\n  operationId: archiveSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files\n  method: post\n  operationId:\
  \ uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/files/{fileToken}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files/{fileToken}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signings/{signingId}/comments\n  method: get\n  operationId: listComments\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signings/{signingId}/comments\n  method: post\n  operationId: addComment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/erasure\n  method: post\n  operationId: eraseSignings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Irreversible bulk purge of terminal signing records.\n- path: /v1/signings/{signingId}/cancel\n  method: post\n  operationId: cancelSigning\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signings/{signingId}/document\n  method: get\n  operationId: downloadSignedDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signings/{signingId}/signers\n  method: post\n  operationId: addSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    human-in-the-loop: required\n    x-curation-reason: Adds a billable signer to a live ceremony and sends them an\
  \ invitation.\n- path: /v1/signings/{signingId}/signers/{signerId}\n  method: patch\n  operationId: updateSignerMethods\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signings/{signingId}/signers/{signerId}\n  method: delete\n  operationId: removeSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signings/{signingId}/signers/{signerId}/remind\n  method: post\n  operationId: remindSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/signings/{signingId}/simulate\n  method: post\n  operationId: simulateSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\ncurated: '2026-08-31'\ncuration_note: 'The mechanical classifier reads HTTP method and keyword only, and returned human_in_the_loop_required:\n  0 for an estate whose writes are legally significant acts. Curated 2026-08-31 against the provider''s own docs\n  and contracts: every operation that opens or completes a national eID identity verification or a qualified electronic\n  signature, every billed trust-service call, and every irreversible erasure now carries human-in-the-loop:\
  \ required,\n  with the reason recorded per operation in x-curation-reason. Signing and signature-requesting operations are additionally\n  raised to consequence: physical because they bind a real person to a legally effective instrument and bill for\n  it. Nothing else in the generated classification was altered.'\nrelated:\n  reversibility: conventions/tvarka-atk-api-conventions.yml + conventions/tvarka-sign-api-conventions.yml\n  mcp: mcp/tvarka-sign-api-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/agentic-access/tvarka-agentic-access.yml
summary_line: 44 operations · 31 acting · 15 human-in-the-loop
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
- Webhook
- Identity
- Trust Services
- GDPR
---
