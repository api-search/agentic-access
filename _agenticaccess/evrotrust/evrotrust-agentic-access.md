---
acting_count: 100
action_class_counts:
  acting: 100
  connected: 4
api_specs:
- filename: evrotrust-all-signing-api-openapi.yml
  format: yaml
  label: Evrotrust All Signing API
  slug: evrotrust-all-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-all-signing-api-openapi.yml
- filename: evrotrust-e-authentication-api-openapi.yml
  format: yaml
  label: Evrotrust E Authentication API
  slug: evrotrust-e-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-authentication-api-openapi.yml
- filename: evrotrust-e-delivery-api-openapi.yml
  format: yaml
  label: Evrotrust E Delivery API
  slug: evrotrust-e-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-delivery-api-openapi.yml
- filename: evrotrust-e-signatures-api-openapi.yml
  format: yaml
  label: Evrotrust E Signatures API
  slug: evrotrust-e-signatures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-signatures-api-openapi.yml
- filename: evrotrust-evrotrust-eid-registered-users-api-openapi.yml
  format: yaml
  label: Evrotrust Evrotrust eID (Registered Users) API
  slug: evrotrust-evrotrust-eid-registered-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-evrotrust-eid-registered-users-api-openapi.yml
- filename: evrotrust-ident-lite-advanced-basic-api-openapi.yml
  format: yaml
  label: Evrotrust Ident Lite (Advanced, Basic) API
  slug: evrotrust-ident-lite-advanced-basic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-ident-lite-advanced-basic-api-openapi.yml
- filename: evrotrust-one-time-signatures-documents-api-openapi.yml
  format: yaml
  label: Evrotrust One-time Signatures (Documents) API
  slug: evrotrust-one-time-signatures-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-one-time-signatures-documents-api-openapi.yml
- filename: evrotrust-one-time-signatures-hash-api-openapi.yml
  format: yaml
  label: Evrotrust One-time Signatures (Hash) API
  slug: evrotrust-one-time-signatures-hash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-one-time-signatures-hash-api-openapi.yml
- filename: evrotrust-signing-via-app-sdk-documents-api-openapi.yml
  format: yaml
  label: Evrotrust Signing via App/SDK (Documents) API
  slug: evrotrust-signing-via-app-sdk-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-signing-via-app-sdk-documents-api-openapi.yml
- filename: evrotrust-signing-via-app-sdk-hash-api-openapi.yml
  format: yaml
  label: Evrotrust Signing via App/SDK (Hash) API
  slug: evrotrust-signing-via-app-sdk-hash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-signing-via-app-sdk-hash-api-openapi.yml
consequence_counts:
  physical: 20
  read: 4
  write: 80
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Evrotrust Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /delivery/online
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/doc/offline/activate/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/doc/offline/activate/resend-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/group/offline/activate/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/group/offline/activate/resend-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/offline/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/offline/withdraw-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/offline/withdraw-1-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/offline/withdraw-1-1-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/offline/withdraw-1-1-1-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/offline/withdraw-1-1-1-1-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /document/withdraw
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/group/offline/activate/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/group/offline/activate/resend-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/group/offline/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/group/offline/send-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/offline/activate/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/offline/activate/resend-1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/offline/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hash/offline/send-1
operation_count: 104
overview: 'Evrotrust exposes 104 API operations that an AI agent could call, of which 100 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 80 write, and 20 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Evrotrust
provider_slug: evrotrust
slug: evrotrust-agentic-access
source_filename: evrotrust-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: generated\nsource: openapi/evrotrust-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 104\n  by_action_class:\n    acting: 100\n    connected: 4\n  by_consequence:\n    write: 80\n    physical: 20\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /certificate/hash/offline/ready\n  method: post\n  operationId: readyOfflineHashCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/online\n  method: post\n  operationId: post_delivery-online\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/receipts/download\n  method: post\n  operationId: post_delivery-receipts-download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /delivery/receipts/status\n  method: post\n  operationId: post_delivery-receipts-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/auth/online\n  method: post\n  operationId: post_document-auth-online\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/identification\n  method: post\n  operationId: post_document-doc-identification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/identification/lpis\n  method: post\n  operationId: post_document-doc-identification-lpis\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/offline\n  method: post\n  operationId: post_document-doc-offline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/offline/activate\n  method: post\n  operationId: post_document-doc-offline-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/offline/activate-1\n\
  \  method: post\n  operationId: post_document-doc-offline-activate-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/offline/activate/resend\n  method: post\n  operationId: post_document-doc-offline-activate-resend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/offline/activate/resend-1\n  method: post\n  operationId: post_document-doc-offline-activate-resend-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/offline/file\n  method: post\n  operationId: post_document-doc-offline-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/doc/offline/refid\n  method: post\n  operationId: post_document-doc-offline-refid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /document/doc/online\n  method: post\n  operationId: post_document-doc-online\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/download\n  method: post\n  operationId: post_document-download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/download-1\n  method: post\n  operationId: post_document-download-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/download-2\n  method: post\n  operationId: post_document-download-2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/download-3\n  method: post\n  operationId: post_document-download-3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/download\n  method: post\n  operationId: post_document-group-download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/download-1\n  method: post\n  operationId: post_document-group-download-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/download-2\n  method: post\n  operationId: post_document-group-download-2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/download-3\n  method: post\n  operationId:\
  \ post_document-group-download-3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/download-3-1\n  method: post\n  operationId: post_document-group-download-3-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/hash/online\n  method: post\n  operationId: post_document-group-hash-online\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline\n  method: post\n  operationId: post_document-group-offline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline/activate\n  method: post\n  operationId: post_document-group-offline-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline/activate-1\n  method: post\n  operationId: post_document-group-offline-activate-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline/activate/resend\n  method: post\n  operationId: post_document-group-offline-activate-resend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline/activate/resend-1\n  method: post\n  operationId: post_document-group-offline-activate-resend-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline/file\n  method: post\n  operationId: post_document-group-offline-file\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline/ready\n  method: post\n  operationId: readyGroupOfflineDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/offline/refid\n  method: post\n  operationId: post_document-group-offline-refid\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/online\n  method: post\n  operationId: post_document-group-online\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/ready\n  method: post\n  operationId: readyGroupDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/status\n\
  \  method: post\n  operationId: post_document-group-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/status-1\n  method: post\n  operationId: post_document-group-status-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/status-2\n  method: post\n  operationId: post_document-group-status-2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/status-3\n  method: post\n  operationId: post_document-group-status-3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/status-4\n  method: post\n  operationId: post_document-group-status-4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/status-5\n  method: post\n  operationId: post_document-group-status-5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/group/terms/offline/download\n  method: post\n  operationId: post_document-group-terms-offline-download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/hash/online\n  method: post\n  operationId: post_document-hash-online\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/offline/ready\n  method:\
  \ post\n  operationId: readyDocumentOffline\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/offline/withdraw\n  method: post\n  operationId: post_document-offline-withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/offline/withdraw-1\n  method: post\n  operationId: post_document-offline-withdraw-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/offline/withdraw-1-1\n  method: post\n  operationId: post_document-offline-withdraw-1-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/offline/withdraw-1-1-1\n  method: post\n  operationId: post_document-offline-withdraw-1-1-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/offline/withdraw-1-1-1-1\n  method: post\n  operationId: post_document-offline-withdraw-1-1-1-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/offline/withdraw-1-1-1-1-1\n  method: post\n  operationId: post_document-offline-withdraw-1-1-1-1-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/ready\n  method:\
  \ post\n  operationId: readyDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/status\n  method: post\n  operationId: post_document-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/status-1\n  method: post\n  operationId: post_document-status-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /document/status-2\n  method: post\n  operationId: post_document-status-2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/status-3\n  method: post\n  operationId: post_document-status-3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/status-4\n  method: post\n  operationId: post_document-status-4\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/status-5\n  method: post\n  operationId: post_document-status-5\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/terms/offline/download\n  method: post\n  operationId: post_document-terms-offline-download\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/thread/status\n  method: post\n  operationId: post_document-thread-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/threads/status\n  method: post\n  operationId: post_document-threads-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /document/withdraw\n  method: post\n  operationId: post_document-withdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /hash/certificate/check\n  method: post\n  operationId: post_hash-certificate-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/certificate/check-1\n  method: post\n  operationId: post_hash-certificate-check-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/certificate/get\n  method: post\n  operationId: post_hash-certificate-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hash/certificate/get-1\n\
  \  method: post\n  operationId: post_hash-certificate-get-1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hash/group/certificate/check\n  method: post\n  operationId: post_hash-group-certificate-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/certificate/check-1\n  method: post\n  operationId: post_hash-group-certificate-check-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/certificate/get\n\
  \  method: post\n  operationId: post_hash-group-certificate-get\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/certificate/get-1\n  method: post\n  operationId: post_hash-group-certificate-get-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/activate\n  method: post\n  operationId: post_hash-group-offline-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/activate-1\n  method: post\n  operationId: post_hash-group-offline-activate-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/activate/resend\n  method: post\n  operationId: post_hash-group-offline-activate-resend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/activate/resend-1\n  method: post\n  operationId:\
  \ post_hash-group-offline-activate-resend-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/check\n  method: post\n  operationId: post_hash-group-offline-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/check-1\n  method: post\n  operationId: post_hash-group-offline-check-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/download\n  method: post\n  operationId: post_hash-offline-download-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/download-1\n  method: post\n  operationId: post_hash-offline-download-1-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/download-2\n  method: post\n  operationId: post_hash-offline-download-1-2\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/download-2-1\n  method: post\n  operationId: post_hash-offline-download-1-2-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/file/init\n  method: post\n  operationId: post_hash-group-offline-file-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /hash/group/offline/init\n  method: post\n  operationId: post_hash-group-offline-init\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/send\n  method: post\n  operationId: post_hash-group-offline-send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/group/offline/send-1\n  method: post\n  operationId: post_hash-group-offline-send-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/offline/activate\n  method: post\n  operationId: post_hash-offline-activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/offline/activate-1\n  method: post\n  operationId: post_hash-offline-activate-1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/offline/activate/resend\n\
  \  method: post\n  operationId: post_hash-offline-activate-resend\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hash/offline/activate/resend-1\n  method: post\n  operationId: post_hash-offline-activate-resend-1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\n\n# --- truncated at 32 KB (37 KB total) ---\n# Full source: https://artifacts.apis.io/evrotrust/agentic-access/evrotrust-agentic-access.yml\n"
source_yaml_url: https://artifacts.apis.io/evrotrust/agentic-access/evrotrust-agentic-access.yml
summary_line: 104 operations · 100 acting
tags:
- Company
- Trust Services
- E-Signature
- Digital Identity
- eIDAS
- KYC
- Identity Verification
- Timestamping
- Compliance
---
