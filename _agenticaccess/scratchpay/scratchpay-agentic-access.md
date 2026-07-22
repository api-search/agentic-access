---
acting_count: 3
action_class_counts:
  acting: 3
api_specs:
- filename: scratchpay-scratchpay-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Borrower Application API
  slug: scratchpay-borrower-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-scratchpay-1.0.0-apis-swagger.yml
- filename: scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Care Credit API
  slug: scratchpay-care-credit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml
- filename: scratchpay-partner-1.0.0-apis-swagger.yml
  format: yaml
  label: Scratchpay Partner Result API
  slug: scratchpay-partner-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/openapi/scratchpay-partner-1.0.0-apis-swagger.yml
consequence_counts:
  physical: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Scratchpay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /application
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /application
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /application/{loanUniqueId}/result
operation_count: 3
overview: 'Scratchpay exposes 3 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Scratchpay
provider_slug: scratchpay
slug: scratchpay-agentic-access
source_filename: scratchpay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/scratchpay-partner-1.0.0-apis-swagger.yml, openapi/scratchpay-scratchpay-1.0.0-apis-swagger.yml,\n  openapi/scratchpay-scratchpay-care-credit-1.0.0-apis-swagger.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    acting: 3\n  by_consequence:\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /application/{loanUniqueId}/result\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /application\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /application\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scratchpay/refs/heads/main/agentic-access/scratchpay-agentic-access.yml
summary_line: 3 operations · 3 acting
tags:
- Company
- Financing
- Payments
- Lending
- Veterinary
- Healthcare
- Fintech
- Buy Now Pay Later
- Point of Sale
---
