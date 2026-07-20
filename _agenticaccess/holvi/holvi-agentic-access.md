---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: holvi-psd2-openapi.yml
  format: yaml
  label: Holvi PSD2 API
  slug: holvi-psd2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holvi/refs/heads/main/openapi/holvi-psd2-openapi.yml
consequence_counts:
  physical: 2
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Holvi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment-initiation/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment-initiation/{payment_initialization_id}/confirm-vop
operation_count: 9
overview: 'Holvi exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Holvi
provider_slug: holvi
slug: holvi-agentic-access
source_filename: holvi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/holvi-psd2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 4\n    connected: 5\n  by_consequence:\n    write: 2\n    read: 5\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/consent/initiate/usernamepassword/\n  method: post\n  operationId: initiateConsentUsernamePassword\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/consent/token/{code}/exchange/\n  method: get\n\
  \  operationId: exchangeConsentToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/payment-accounts/\n  method: get\n  operationId: listPaymentAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/payment-accounts/{uuid}/\n  method: get\n  operationId: getPaymentAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/payment-accounts/{uuid}/payments/\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/payment-accounts/{payment_account_uuid}/payments/{payment_uuid}/\n  method: get\n  operationId:\
  \ getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/payment-initiation/\n  method: post\n  operationId: initiatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/payment-initiation/{payment_initialization_id}/confirm-vop\n  method: post\n  operationId: confirmVop\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v2/renew-certificate/\n  method: post\n  operationId: renewCertificate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holvi/refs/heads/main/agentic-access/holvi-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Company
- Banking
- Fintech
- Payments
- Business Banking
- PSD2
- Open Banking
- SEPA
- Finland
---
