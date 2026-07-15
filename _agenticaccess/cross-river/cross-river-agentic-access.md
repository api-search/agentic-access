---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 6
api_specs:
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Accounts API
  slug: cross-river-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River ACH Payments API
  slug: cross-river-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Wires API
  slug: cross-river-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Instant Payments API
  slug: cross-river-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Cards API
  slug: cross-river-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Lending API
  slug: cross-river-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
- filename: cross-river-openapi.yml
  format: yaml
  label: Cross River Customer Management API
  slug: cross-river-customer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/openapi/cross-river-openapi.yml
consequence_counts:
  physical: 5
  read: 6
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cross River Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ach/v1/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /core/v1/dda/accounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rtp/v1/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wires/v1/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /wires/v1/payments/{id}/cancel
operation_count: 22
overview: 'Cross River exposes 22 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 11 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cross River
provider_slug: cross-river
slug: cross-river-agentic-access
source_filename: cross-river-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cross-river-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 16\n    connected: 6\n  by_consequence:\n    write: 11\n    read: 6\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /core/v1/cm/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/cm/customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/v1/cm/customers/{id}\n  method: delete\n  operationId: deactivateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/cm/customers/{customerId}/beneficial-owners\n  method: post\n  operationId: addBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/cm/customers/{customerId}/identifications\n  method: post\n  operationId: addIdentification\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/dda/accounts\n  method: post\n  operationId: createAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/dda/accounts/{accountNumber}/restrictions\n  method: post\n  operationId: addAccountRestriction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /core/v1/dda/accounts/{accountNumber}/statements\n  method: get\n  operationId: listAccountStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ach/v1/payments\n  method: post\n  operationId: sendAchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wires/v1/payments\n  method: post\n  operationId: sendWirePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wires/v1/payments/{id}/cancel\n  method: post\n  operationId: cancelWirePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/v1/payments\n  method: post\n  operationId: sendInstantPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rtp/v1/directory\n  method: get\n\
  \  operationId: getInstantPaymentDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardmanagement/v1/cards\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardmanagement/v1/cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardmanagement/v1/cards/{id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardmanagement/v1/cards/{id}/activate\n\
  \  method: post\n  operationId: activateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardmanagement/v1/cards/{id}/suspend\n  method: post\n  operationId: suspendCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cardmanagement/v1/cards/{id}/close\n  method: post\n  operationId: closeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /loan\n  method: post\n  operationId: addLoan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /loandetail/{id}\n  method: get\n  operationId: getLoanDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /loan/{id}/fundinginfo\n  method: put\n  operationId: requestLoanFundingRails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cross-river/refs/heads/main/agentic-access/cross-river-agentic-access.yml
summary_line: 22 operations · 16 acting
tags:
- Embedded Finance
- Banking as a Service
- BaaS
- Payments
- ACH
- Wire
- Push-to-Card
- Lending
- Accounts
- Cards
- Fintech
- RTP
- FedNow
---
