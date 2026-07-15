---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 3
api_specs:
- filename: pitney-bowes-openapi.yml
  format: yaml
  label: Pitney Bowes APIs
  slug: pitney-bowes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pitney-bowes/refs/heads/main/openapi/pitney-bowes-openapi.yml
consequence_counts:
  physical: 7
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pitney Bowes Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shippingservices/v1/addresses/verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shippingservices/v1/manifests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shippingservices/v1/pickups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /shippingservices/v1/pickups/{pickupId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shippingservices/v1/rates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /shippingservices/v1/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /shippingservices/v1/shipments/{shipmentId}
operation_count: 11
overview: 'Pitney Bowes exposes 11 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 1 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pitney Bowes
provider_slug: pitney-bowes
slug: pitney-bowes-agentic-access
source_filename: pitney-bowes-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/pitney-bowes-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 8\n    connected: 3\n  by_consequence:\n    write: 1\n    physical: 7\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: getOAuthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/rates\n  method: post\n  operationId: rateParcel\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/shipments\n  method: post\n  operationId: createShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/shipments/{shipmentId}\n  method: get\n  operationId: reprintShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /shippingservices/v1/shipments/{shipmentId}\n\
  \  method: delete\n  operationId: voidShipment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/manifests\n  method: post\n  operationId: createManifest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/tracking/{trackingNumber}\n  method: get\n  operationId: trackParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /shippingservices/v1/addresses/verify\n  method: post\n  operationId: verifyAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/pickups\n  method: post\n  operationId: schedulePickup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/pickups/{pickupId}\n  method: delete\n  operationId: cancelPickup\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /shippingservices/v1/ledger/transactions/reports\n  method: get\n  operationId: getTransactionReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pitney-bowes/refs/heads/main/agentic-access/pitney-bowes-agentic-access.yml
summary_line: 11 operations · 8 acting
tags:
- Mailing
- Shipping
- Fortune 1000
---
