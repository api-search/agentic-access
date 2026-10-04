---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: autofi-authorization-api-openapi.yml
  format: yaml
  label: AutoFi Authorization API
  slug: autofi-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-authorization-api-openapi.yml
- filename: autofi-calculate-payment-api-openapi.yml
  format: yaml
  label: AutoFi Calculate Payment API
  slug: autofi-calculate-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-calculate-payment-api-openapi.yml
- filename: autofi-dealers-api-openapi.yml
  format: yaml
  label: AutoFi Dealers API
  slug: autofi-dealers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-dealers-api-openapi.yml
- filename: autofi-dealmaker-api-openapi.yml
  format: yaml
  label: AutoFi Dealmaker API
  slug: autofi-dealmaker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-dealmaker-api-openapi.yml
- filename: autofi-loan-applications-api-openapi.yml
  format: yaml
  label: AutoFi Loan Applications API
  slug: autofi-loan-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-loan-applications-api-openapi.yml
- filename: autofi-prequalification-api-openapi.yml
  format: yaml
  label: AutoFi Prequalification API
  slug: autofi-prequalification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/openapi/autofi-prequalification-api-openapi.yml
consequence_counts:
  physical: 3
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Autofi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/estimate/cash
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/estimate/finance
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/estimate/lease
operation_count: 11
overview: 'AutoFi exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 5 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AutoFi
provider_slug: autofi
slug: autofi-agentic-access
source_filename: autofi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/autofi-authorization-api-openapi.yml, openapi/autofi-calculate-payment-api-openapi.yml,\n  openapi/autofi-dealers-api-openapi.yml, openapi/autofi-dealmaker-api-openapi.yml, openapi/autofi-loan-applications-api-openapi.yml,\n  openapi/autofi-prequalification-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 8\n    connected: 3\n  by_consequence:\n    write: 5\n    physical: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/token\n  method: post\n  operationId: postAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/estimate/cash\n  method: post\n  operationId: postV1EstimateCash\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - create:estimate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/estimate/finance\n  method: post\n  operationId: postV1EstimateFinance\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - create:estimate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v1/estimate/lease\n  method: post\n  operationId: postV1EstimateLease\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - create:estimate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dealer/lookup\n  method: post\n  operationId: postV1DealerLookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - lookup:dealers\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dealmaker\n  method: post\n  operationId: postV1Dealmaker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create:dealmaker\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/dealmaker/credit-application\n  method: post\n  operationId: postV1DealmakerCreditApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create:dealmakercredit\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loan-application\n  method: post\n  operationId: postV1LoanApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create:loanapplications\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/loan-application/{loanApplicationId}\n  method:\
  \ get\n  operationId: getV1LoanApplicationByLoanApplicationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:loanapplications\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loan-application/{loanApplicationId}/externalResources\n  method: get\n  operationId: getV1LoanApplicationByLoanApplicationIdExternalResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:loanapplications\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/prequalification\n  method: post\n  operationId: postV1Prequalification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - create:prequalification\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autofi/refs/heads/main/agentic-access/autofi-agentic-access.yml
summary_line: 11 operations · 8 acting
tags:
- Company
- Automotive
- Fintech
- Digital Retail
- Auto Finance
- Dealership
- Sales Enablement
- Software-as-a-Service
- Lending
- Loan Origination
- Credit Decisioning
- Payment Calculation
- Prequalification
---
