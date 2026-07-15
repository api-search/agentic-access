---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 13
api_specs:
- filename: allianz-trade-payment-overdues.yaml
  format: yaml
  label: Allianz Trade Payment Overdues API
  slug: payment-overdues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-payment-overdues.yaml
- filename: allianz-trade-company-grade.yaml
  format: yaml
  label: Allianz Trade Company Grade API
  slug: company-grade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-company-grade.yaml
- filename: allianz-trade-claims.yaml
  format: yaml
  label: Allianz Trade Claims API
  slug: claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-claims.yaml
- filename: allianz-trade-policy.yaml
  format: yaml
  label: Allianz Trade Policy API
  slug: policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-policy.yaml
consequence_counts:
  physical: 4
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Allianz Trade Online Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /claims
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /company-grades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /overdues
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policies/{policyId}/joint-insureds
operation_count: 17
overview: 'Allianz Trade exposes 17 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Allianz Trade
provider_slug: allianz-trade-online
slug: allianz-trade-online-agentic-access
source_filename: allianz-trade-online-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/allianz-trade-claims.yaml, openapi/allianz-trade-company-grade.yaml, openapi/allianz-trade-payment-overdues.yaml,\n  openapi/allianz-trade-policy.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 13\n    acting: 4\n  by_consequence:\n    read: 13\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /claims\n  method: get\n  operationId: listClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims\n  method: post\n  operationId: submitClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claimId}\n  method: get\n  operationId: getClaim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company-grades\n  method: get\n  operationId: listCompanyGrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company-grades\n  method: post\n  operationId: requestCompanyGrade\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /company-grades/{gradeId}\n  method: get\n  operationId: getCompanyGrade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /overdues\n  method: get\n  operationId: listOverdues\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /overdues\n  method: post\n  operationId:\
  \ reportOverdue\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /overdues/{overdueId}\n  method: get\n  operationId: getOverdue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{jobId}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies\n  method: get\n  operationId: listPolicies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies/{policyId}\n\
  \  method: get\n  operationId: getPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies/{policyId}/joint-insureds\n  method: get\n  operationId: listJointInsureds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policies/{policyId}/joint-insureds\n  method: post\n  operationId: addJointInsured\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs/{jobId}\n  method: get\n  operationId: getJobStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/agentic-access/allianz-trade-online-agentic-access.yml
summary_line: 17 operations · 4 acting
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
---
