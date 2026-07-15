---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: mastercard-gateway-api-openapi.yml
  format: yaml
  label: Mastercard Gateway API
  slug: mastercard-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastercard-gateway-api/refs/heads/main/openapi/mastercard-gateway-api-openapi.yml
consequence_counts:
  physical: 5
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mastercard Gateway Api Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchant/{merchantId}/hostedCheckout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /merchant/{merchantId}/order/{orderid}/transaction/{transactionid}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchant/{merchantId}/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /merchant/{merchantId}/token/{tokenId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /merchant/{merchantId}/token/{tokenId}
operation_count: 14
overview: 'Mastercard Gateway API exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 4 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mastercard Gateway API
provider_slug: mastercard-gateway-api
slug: mastercard-gateway-api-agentic-access
source_filename: mastercard-gateway-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mastercard-gateway-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 9\n    connected: 5\n  by_consequence:\n    physical: 5\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /merchant/{merchantId}/order/{orderid}/transaction/{transactionid}\n  method: put\n  operationId: transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /merchant/{merchantId}/order/{orderid}/transaction/{transactionid}\n  method: get\n  operationId: retrieveTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{merchantId}/order/{orderid}\n  method: get\n  operationId: retrieveOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{merchantId}/session\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchantId}/session/{sessionId}\n  method: put\n  operationId: updateSession\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchantId}/session/{sessionId}\n  method: get\n  operationId: retrieveSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{merchantId}/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchantId}/token/{tokenId}\n  method: put\n  operationId: createOrUpdateToken\n \
  \ x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchantId}/token/{tokenId}\n  method: get\n  operationId: retrieveToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant/{merchantId}/token/{tokenId}\n  method: delete\n  operationId: deleteToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /merchant/{merchantId}/3DSecureId/{3DSecureId}\n  method: put\n  operationId: threeDSecure\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchantId}/hostedCheckout\n  method: post\n  operationId: hostedCheckoutInitiate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchantId}/batch/{batchId}\n  method: put\n  operationId: batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchant/{merchantId}/gatewayStatus\n  method: get\n  operationId: checkGateway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastercard-gateway-api/refs/heads/main/agentic-access/mastercard-gateway-api-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Credit Cards
- Gateway
- Payment Processing
- Payments
---
