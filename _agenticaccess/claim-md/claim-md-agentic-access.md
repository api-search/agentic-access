---
acting_count: 15
action_class_counts:
  acting: 15
api_specs:
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Claim Submission API
  slug: claim-submission
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Claim Status API
  slug: claim-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD ERA / Remits API
  slug: era-remits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Eligibility API
  slug: eligibility
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
- filename: claim-md-openapi.yml
  format: yaml
  label: Claim.MD Responses & Files API
  slug: responses-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/openapi/claim-md-openapi.yml
consequence_counts:
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Claim Md Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Claim.MD exposes 15 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Claim.MD
provider_slug: claim-md
slug: claim-md-agentic-access
source_filename: claim-md-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/claim-md-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 15\n  by_consequence:\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /services/upload/\n  method: post\n  operationId: uploadClaims\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/uploadlist/\n  method: post\n  operationId: listUploads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/response/\n  method: post\n  operationId: getClaimResponses\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/modify/\n  method: post\n  operationId: getClaimModifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/notes/\n  method: post\n  operationId: getClaimNotes\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/archive/\n  method: post\n  operationId: archiveClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/eralist/\n  method: post\n  operationId: listEra\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/era835/\n  method: post\n  operationId:\
  \ getEra835\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/eradata/\n  method: post\n  operationId: getEraData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/erapdf/\n  method: post\n  operationId: getEraPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/elig/\n\
  \  method: post\n  operationId: submitEligibility270\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/eligdata/\n  method: post\n  operationId: submitEligibilityData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/payerlist/\n  method: post\n  operationId: listPayers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /services/enroll/\n  method: post\n  operationId: requestEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /services/appeal/\n  method: post\n  operationId: requestAppeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claim-md/refs/heads/main/agentic-access/claim-md-agentic-access.yml
summary_line: 15 operations · 15 acting
tags:
- Healthcare
- Medical Claims
- Clearinghouse
- EDI
- X12
- Revenue Cycle
---
