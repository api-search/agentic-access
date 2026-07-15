---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: openapi.yaml
  format: yaml
  label: EchoSync Partner-Connect API
  slug: echosync-partner-connect-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis/echogl/rest-api/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Customer API
  slug: echosync-customer-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Customer_API_OAuth_Public/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Carrier API
  slug: echosync-carrier-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Carrier_API_Public/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Authorizer API
  slug: echosync-authorizer-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Echo_Authorizer_Public/
consequence_counts:
  physical: 5
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Echo Global Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/query/shipments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/rates/LTL
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/shipments/LTL
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/shipments/PL
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/shipments/TL
operation_count: 14
overview: 'Echo Global Logistics exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Echo Global Logistics
provider_slug: echo-global
slug: echo-global-agentic-access
source_filename: echo-global-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/echosync-authorizer-api.json, openapi/echosync-customer-api.json, openapi/echosync-partner-connect-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 7\n    connected: 7\n  by_consequence:\n    write: 2\n    read: 7\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/__health\n  method: get\n\
  \  operationId: Health.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/quotes/{id}\n  method: get\n  operationId: Quote_v2.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/quotes\n  method: post\n  operationId: Quote_v2.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ping\n  method: get\n  operationId: GetPingResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/shipments/LTL\n  method: post\n  operationId:\
  \ CreateShipmentLTL\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/shipments/TL\n  method: post\n  operationId: CreateShipmentTL\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/shipments/PL\n  method: post\n  operationId: CreateShipmentPL\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/shipments/{Id}\n  method: get\n  operationId: GetShipment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/shipments/{Id}/status\n  method: get\n  operationId: GetShipmentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/shipments/{Id}/tracking\n  method: get\n  operationId: GetShipmentTracking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/shipments/{Id}/documents\n  method: get\n  operationId: GetShipmentDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/rates/LTL\n  method: post\n  operationId: GetShipmentRatesLTL\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/query/shipments\n  method: post\n  operationId: QueryShipments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/agentic-access/echo-global-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Freight
- Logistics
- Shipping
- LTL
- Truckload
- Freight Brokerage
- Transportation
- Supply Chain
---
