---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: credgenics-recovery-openapi.yml
  format: yaml
  label: Credgenics Recovery API
  slug: credgenics-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credgenics/refs/heads/main/openapi/credgenics-recovery-openapi.yml
consequence_counts:
  physical: 1
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Credgenics Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /recovery/payments/{loan_id}
operation_count: 7
overview: 'Credgenics exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Credgenics
provider_slug: credgenics
slug: credgenics-agentic-access
source_filename: credgenics-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/credgenics-recovery-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /user/public/access-token\n  method: post\n  operationId: createAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recovery/v1/loans/{loan_id}\n  method: get\n  operationId: getLoan\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recovery/v1/loan/{loan_id}\n  method: post\n  operationId: uploadLoan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recovery/v1/loan/{loan_id}\n  method: patch\n  operationId: updateLoan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recovery/payments/{loan_id}\n  method: patch\n  operationId: updatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recovery/v1/customers/{customer_id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recovery/loan/{transaction_id}\n  method: post\n  operationId: uploadTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credgenics/refs/heads/main/agentic-access/credgenics-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- Company
- Enterprise
- Financial Services
- Debt Collection
- Loan Recovery
- Lending
- Collections
- Fintech
- India
---
