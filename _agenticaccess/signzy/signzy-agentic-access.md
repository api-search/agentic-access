---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: signzy-authentication-api-openapi.yml
  format: yaml
  label: Signzy Authentication API
  slug: signzy-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-authentication-api-openapi.yml
- filename: signzy-banking-api-openapi.yml
  format: yaml
  label: Signzy Banking API
  slug: signzy-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-banking-api-openapi.yml
- filename: signzy-identity-india-api-openapi.yml
  format: yaml
  label: Signzy Identity (India) API
  slug: signzy-identity-india-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-identity-india-api-openapi.yml
- filename: signzy-identity-us-api-openapi.yml
  format: yaml
  label: Signzy Identity (US) API
  slug: signzy-identity-us-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/openapi/signzy-identity-us-api-openapi.yml
consequence_counts:
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. Signzy operations touch PII, biometric, and financial identity data, so most write operations should require a subject, tight token TTLs, and audit. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Signzy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Signzy exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Signzy
provider_slug: signzy
slug: signzy-agentic-access
source_filename: signzy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/signzy-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. Signzy operations touch PII, biometric, and financial identity data,\n  so most write operations should require a subject, tight token TTLs, and audit. See\n  research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 5\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/customers/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    note: Issues an access token; treat credentials as high-value secrets.\n- path: /api/customers/logout\n\
  \  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    audit: required\n- path: /api/v3/aadhaar/verify\n  method: post\n  operationId: verifyAadhaar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 600\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n      - pii\n    audit: required\n    note: Processes Indian national-ID PII; requires explicit end-user consent.\n- path: /api/v3/pan/simple\n  method: post\n  operationId: verifyPan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 600\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n      - pii\n    audit:\
  \ required\n    note: Processes Indian tax-identity PII; requires explicit end-user consent.\n- path: /api/v3/us/document-intelligence-advance\n  method: post\n  operationId: usDocumentIntelligenceAdvance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 600\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n      - pii\n    audit: required\n    note: Processes US identity-document images and biometric-adjacent data.\n- path: /api/v3/underwriting/get-passbook-otp\n  method: post\n  operationId: getPassbookOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 600\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    note: Triggers an OTP against a real bank account;\
  \ guard against abuse.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signzy/refs/heads/main/agentic-access/signzy-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Identity Verification
- KYC
- KYB
- AML
- Onboarding
- Compliance
- RegTech
---
