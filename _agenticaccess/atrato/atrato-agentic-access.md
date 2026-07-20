---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: atrato-partners-openapi.yml
  format: yaml
  label: Atrato Partners API
  slug: atrato-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atrato/refs/heads/main/openapi/atrato-partners-openapi.yml
consequence_counts:
  physical: 3
  read: 7
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Atrato Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v4/ecommerce/integration/{partner-key}/order/{order-id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v4/ecommerce/integration/{partner-key}/order/{order-id}/delivery
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v4/integration/cash-in/register-payment
operation_count: 13
overview: 'Atrato exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 3 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Atrato
provider_slug: atrato
slug: atrato-agentic-access
source_filename: atrato-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/atrato-partners-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    write: 3\n    read: 7\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v4/integration/login\n  method: post\n  operationId: autenticación\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/integration/cash-in/search\n  method: get\n  operationId: get_api-v4-integration-cash-in-search\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/integration/cash-in/available-stores\n  method: get\n  operationId: get_api-v4-integration-cash-in-available-stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/integration/cash-in/register-payment\n  method: post\n  operationId: post_api-v4-integration-cash-in-register-payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/integration/cash-in/payments\n  method: get\n  operationId: get_api-v4-integration-cash-in-payments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/integration/cash-in/payment-details/{paymentId}\n  method: get\n  operationId: get_api-v4-integration-cash-in-payment-details-paymentid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/ecommerce/integration/{partner-key}/login\n  method: post\n  operationId: obtener-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/ecommerce/integration/{partner-key}/application\n  method: post\n  operationId: generar-orden\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/ecommerce/integration/{partner-key}/order/{order-id}\n  method: get\n  operationId: consulta-de-orden\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/ecommerce/integration/{partner-key}/order/{order-id}/delivery\n  method: post\n  operationId: registrar-entrega\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/ecommerce/integration/{partner-key}/order/{order-id}/cancel\n\
  \  method: post\n  operationId: solicitar-cancelacion\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v4/ecommerce/integration/{partner-key}/disbursement\n  method: get\n  operationId: consulta-de-desembolsos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v4/ecommerce/integration/{partner-key}/disbursement/{transaction-id}\n  method: get\n  operationId: consulta-de-desembolsos-orden\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atrato/refs/heads/main/agentic-access/atrato-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Company
- Fintech
- Payments
- Buy Now Pay Later
- Lending
- Mexico
- Point of Sale
- Ecommerce
---
