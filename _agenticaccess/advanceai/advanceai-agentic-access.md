---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: advanceai-authentication-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Authentication API
  slug: advanceai-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-authentication-api-openapi.yml
- filename: advanceai-document-verification-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Document Verification API
  slug: advanceai-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-document-verification-api-openapi.yml
- filename: advanceai-face-comparison-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Face Comparison API
  slug: advanceai-face-comparison-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-face-comparison-api-openapi.yml
- filename: advanceai-liveness-detection-api-openapi.yml
  format: yaml
  label: ADVANCE.AI Liveness Detection API
  slug: advanceai-liveness-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-liveness-detection-api-openapi.yml
consequence_counts:
  read: 4
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Advanceai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'ADVANCE.AI exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ADVANCE.AI
provider_slug: advanceai
slug: advanceai-agentic-access
source_filename: advanceai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/advanceai-authentication-api-openapi.yml, openapi/advanceai-document-verification-api-openapi.yml,\n  openapi/advanceai-face-comparison-api-openapi.yml, openapi/advanceai-liveness-detection-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 5\n    connected: 4\n  by_consequence:\n    write: 5\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /openapi/auth/ticket/v1/generate-token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intl/openapi/face-identity/document-verification/v1/auth-license\n  method: post\n  operationId: authorizeDocumentVerificationLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intl/openapi/face-identity/document-verification/v1/query\n  method: post\n  operationId: queryDocumentVerificationResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi/face-recognition/v4/check\n  method: post\n  operationId: compareFaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /liveness/ext/v1/generate-signature-id\n  method: post\n  operationId: generateLivenessSignatureId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/liveness/v1/auth-license\n  method: post\n  operationId: authorizeLivenessLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/liveness/v3/detection-result\n  method: post\n  operationId: getLivenessDetectionResult\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liveness/ext/v1/get-video\n  method: get\n  operationId: getLivenessVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /liveness/ext/v1/clear-data\n  method: get\n  operationId: clearLivenessPiiData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/agentic-access/advanceai-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- Company
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Face Recognition
- Liveness Detection
- OCR
- Document Verification
- Risk Management
- Artificial Intelligence
- Fintech
- Singapore
---
