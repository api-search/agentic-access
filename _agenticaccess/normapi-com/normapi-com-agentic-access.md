---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: normapi-com-openapi.yml
  format: yaml
  label: NormAPI REST API
  slug: normapi-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normapi-com/openapi/normapi-com-openapi.yml
consequence_counts:
  physical: 6
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Normapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/parse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/parse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/validate
operation_count: 14
overview: 'NormAPI exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 3 write, and 6 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: NormAPI
provider_slug: normapi-com
slug: normapi-com-agentic-access
source_filename: normapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: generated\nsource: openapi/normapi-com-customers-api-openapi.yml, openapi/normapi-com-generation-api-openapi.yml,\n  openapi/normapi-com-invoices-api-openapi.yml, openapi/normapi-com-parse-api-openapi.yml, openapi/normapi-com-parsing-api-openapi.yml,\n  openapi/normapi-com-rules-api-openapi.yml, openapi/normapi-com-validate-api-openapi.yml, openapi/normapi-com-validation-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 5\n    acting: 9\n  by_consequence:\n    read: 5\n    write: 3\n    physical: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/customers\n  method: get\n  operationId: getV1Customers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer}\n  method: get\n  operationId: getV1CustomersByCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{customer}/allowance\n  method: put\n  operationId: putV1CustomersByCustomerAllowance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{customer}/allowance\n  method: delete\n  operationId: deleteV1CustomersByCustomerAllowance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/invoices\n  method: post\n  operationId: postV1Invoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoices\n  method: post\n  operationId: generateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parse\n  method: post\n  operationId: parseInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parse\n  method: post\n  operationId: postV1Parse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules/{code}\n  method: get\n  operationId: getRule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/validate\n  method: post\n  operationId: validateInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/validate\n  method: post\n  operationId: postV1Validate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules/{code}\n  method: get\n  operationId: getV1RulesByCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/normapi-com/agentic-access/normapi-com-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Company
- E-Invoicing
- XRechnung
- ZUGFeRD
- Germany
---
