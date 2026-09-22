---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: enfuce-authorisation-request-api-api-openapi.yml
  format: yaml
  label: Enfuce Authorisation Request API
  slug: enfuce-authorisation-request-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-authorisation-request-api-api-openapi.yml
- filename: enfuce-create-card-api-openapi.yml
  format: yaml
  label: Enfuce Create Card API
  slug: enfuce-create-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-create-card-api-openapi.yml
- filename: enfuce-create-pin-control-access-token-api-openapi.yml
  format: yaml
  label: Enfuce Create PIN Control access token API
  slug: enfuce-create-pin-control-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-create-pin-control-access-token-api-openapi.yml
- filename: enfuce-get-card-api-openapi.yml
  format: yaml
  label: Enfuce Get card API
  slug: enfuce-get-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-get-card-api-openapi.yml
- filename: enfuce-get-card-payment-info-api-openapi.yml
  format: yaml
  label: Enfuce Get Card Payment Info API
  slug: enfuce-get-card-payment-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-get-card-payment-info-api-openapi.yml
- filename: enfuce-get-plastic-manufacturing-history-api-openapi.yml
  format: yaml
  label: Enfuce Get plastic manufacturing history API
  slug: enfuce-get-plastic-manufacturing-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-get-plastic-manufacturing-history-api-openapi.yml
- filename: enfuce-update-card-api-openapi.yml
  format: yaml
  label: Enfuce Update card API
  slug: enfuce-update-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/openapi/enfuce-update-card-api-openapi.yml
consequence_counts:
  physical: 2
  read: 3
  safety-critical: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Enfuce Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/cards/{id}/controlToken
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/cards/{id}/pinControl
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cards/{id}/encrypt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/cards/{id}/reorder-pin
operation_count: 12
overview: 'Enfuce exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 5 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Enfuce
provider_slug: enfuce
slug: enfuce-agentic-access
source_filename: enfuce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: generated\nsource: openapi/card.openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 9\n    connected: 3\n  by_consequence:\n    write: 5\n    read: 3\n    physical: 2\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards\n  method: get\n  operationId: getCards\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{id}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{id}\n  method: patch\n  operationId: patchCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{id}/replace\n  method: post\n  operationId: replaceCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/cards/{id}/reissue\n  method: post\n  operationId: reissueCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{id}/activate\n  method: post\n  operationId: activateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{id}/reorder-pin\n  method: post\n  operationId: reorderPin\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{id}/manufacturing-history\n  method: get\n  operationId: manufacturingHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cards/{id}/encrypt\n  method: post\n  operationId: encryptCardPaymentInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cards/{id}/controlToken\n  method: post\n  operationId: getCardDataControlToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/cards/{id}/pinControl\n  method: post\n  operationId: createPinControl\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enfuce/refs/heads/main/agentic-access/enfuce-agentic-access.yml
summary_line: 12 operations · 9 acting · 2 human-in-the-loop
tags:
- Company
- Payments
- Card Issuing
- FinTech
- API Platform
---
