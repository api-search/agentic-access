---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 3
api_specs:
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Eligibility Inquiry API
  slug: eligibility-inquiry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Eligibility Summary API
  slug: eligibility-summary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Batch Eligibility API
  slug: batch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Claim Status API
  slug: claim-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Payers API
  slug: payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
- filename: pverify-openapi.yml
  format: yaml
  label: pVerify Estimation API
  slug: estimation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-openapi.yml
consequence_counts:
  read: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pverify Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'pVerify exposes 10 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: pVerify
provider_slug: pverify
slug: pverify-agentic-access
source_filename: pverify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pverify-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 7\n    connected: 3\n  by_consequence:\n    write: 7\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /Token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/EligibilitySummary\n  method: post\n  operationId: eligibilitySummary\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/EligibilityInquiry\n  method: post\n  operationId: eligibilityInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetEligibilityResponse\n  method: get\n  operationId: getEligibilityResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/GetPendingInquiries\n  method: get\n  operationId: getPendingInquiries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /API/CancelTransaction\n  method: post\n  operationId: cancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/BatchEligibility\n  method: post\n  operationId: batchEligibility\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/ClaimStatus\n  method: post\n  operationId: claimStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/Payers\n  method: get\n  operationId: getPayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/EstimationInquiry\n  method: post\n  operationId: estimationInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/agentic-access/pverify-agentic-access.yml
summary_line: 10 operations · 7 acting
tags:
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- 270/271
---
