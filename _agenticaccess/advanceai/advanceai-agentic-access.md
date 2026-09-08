---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 1
api_specs:
- filename: advanceai-openapi.yml
  format: yaml
  label: ADVANCE.AI Open API
  slug: advanceai-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/openapi/advanceai-openapi.yml
consequence_counts:
  destructive: 1
  read: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated+corrected
name: Advanceai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'ADVANCE.AI exposes 9 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 7 write.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ADVANCE.AI
provider_slug: advanceai
slug: advanceai-agentic-access
source_filename: advanceai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: generated+corrected\nsource: openapi/advanceai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 8\n    connected: 1\n  by_consequence:\n    write: 7\n    read: 1\n    destructive: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /openapi/auth/ticket/v1/generate-token\n  method: post\n  operationId: generateAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intl/openapi/face-identity/document-verification/v1/auth-license\n\
  \  method: post\n  operationId: authorizeDocumentVerificationLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intl/openapi/face-identity/document-verification/v1/query\n  method: post\n  operationId: queryDocumentVerificationResult\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/face-recognition/v4/check\n  method: post\n  operationId: compareFaces\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /liveness/ext/v1/generate-signature-id\n  method: post\n  operationId: generateLivenessSignatureId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/liveness/v1/auth-license\n  method: post\n  operationId: authorizeLivenessLicense\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi/liveness/v3/detection-result\n  method: post\n  operationId: getLivenessDetectionResult\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /liveness/ext/v1/get-video\n  method: get\n  operationId: getLivenessVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: required\n    token:\n      max-ttl: 900\n    audit: required\n    data-sensitivity: biometric\n    note: Returns a link to biometric video of an identified person. Reads of this class should be audited.\n- path: /liveness/ext/v1/clear-data\n  method: get\n  operationId: clearLivenessPiiData\n  x-agentic-access:\n    action-class: acting\n    consequence: destructive\n    reversible: false\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - always\n      reason: Irreversible.\
  \ ADVANCE.AI documents no restore, no soft delete and no recovery window.\n    audit: required\n    note: Implemented as GET but deletes data. See conventions/advanceai-conventions.yml reversibility.\nx-manual-correction:\n  date: '2026-09-07'\n  by: API Evangelist enrichment pass\n  reason: The heuristic classifies by HTTP method, and ADVANCE.AI implements two consequential operations\n    as GET. clearLivenessPiiData permanently deletes the PII held for a liveness detection and was auto-classified\n    consequence:read / audit:none / no escalation — the most dangerous possible misreading, since it would\n    tell an agent an irreversible deletion is a safe read. getLivenessVideo returns biometric video and\n    was likewise classified as an unaudited read. Both entries below were corrected by hand from https://doc.advance.ai/liveness_detection.html.\n  corrected_operations:\n  - clearLivenessPiiData\n  - getLivenessVideo\n  caveat: A GET that mutates is invisible to method-based classification.\
  \ Any other provider in this catalog\n    that deletes over GET carries the same silent defect.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanceai/refs/heads/main/agentic-access/advanceai-agentic-access.yml
summary_line: 9 operations · 8 acting · 1 human-in-the-loop
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
