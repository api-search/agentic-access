---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 2
api_specs:
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge KYC OCR API
  slug: hyperverge-kyc-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Database Verification API
  slug: hyperverge-database-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Input Validation API
  slug: hyperverge-input-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Matching API
  slug: hyperverge-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
- filename: hyperverge-openapi.yml
  format: yaml
  label: HyperVerge Face Match API
  slug: hyperverge-face-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/openapi/hyperverge-openapi.yml
consequence_counts:
  read: 2
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hyperverge Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'HyperVerge exposes 18 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HyperVerge
provider_slug: hyperverge
slug: hyperverge-agentic-access
source_filename: hyperverge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/hyperverge-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 16\n    connected: 2\n  by_consequence:\n    write: 16\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /readKYC\n  method: post\n  operationId: readKYC\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /readPAN\n  method: post\n  operationId: readPAN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /readAadhaar\n  method: post\n  operationId: readAadhaar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /readPassport\n  method: post\n  operationId: readPassport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /readVoterID\n  method: post\n  operationId: readVoterID\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api\n  method: get\n  operationId: verifyHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/verifyPAN\n  method: post\n  operationId: verifyPAN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/getNameFromPAN\n  method: post\n  operationId: getNameFromPAN\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkDL\n  method: post\n  operationId: checkDL\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkVoterId\n  method: post\n  operationId: checkVoterId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/checkBankAccount\n  method: post\n  operationId: checkBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validatePANInput\n  method: post\n  operationId: validatePANInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validateAadhaarInput\n  method: post\n  operationId: validateAadhaarInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validatePassportInput\n  method: post\n  operationId: validatePassportInput\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/validateVoterIdInput\n  method: post\n  operationId: validateVoterIdInput\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/matchFields\n  method: post\n  operationId: matchFields\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/photo/verifyPair\n\
  \  method: get\n  operationId: faceMatchHealthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/photo/verifyPair\n  method: post\n  operationId: verifyPair\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperverge/refs/heads/main/agentic-access/hyperverge-agentic-access.yml
summary_line: 18 operations · 16 acting
tags:
- Identity Verification
- KYC
- Face Authentication
- Liveness
- Document Verification
- India
- AML
- Onboarding
- Fraud Prevention
- AI
---
