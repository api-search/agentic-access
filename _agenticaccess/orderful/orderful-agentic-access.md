---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 9
api_specs:
- filename: orderful-openapi-original.yml
  format: yaml
  label: Orderful API (Mosaic / v3)
  slug: orderful-api-mosaic-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-openapi-original.yml
consequence_counts:
  read: 9
  safety-critical: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 12
kind: agentic-access
layout: agentic-access
method: generated
name: Orderful Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transactions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transactions/{transactionId}/deliveries/{deliveryId}/accept
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /transactions/{transactionId}/deliveries/{deliveryId}/fail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/convert
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/deliveries/{deliveryId}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/deliveries/{deliveryId}/fail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/labels
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/polling-buckets/{id}/confirm-retrieval
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/transactions
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/transactions/confirm-delivery
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/transactions/raw
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/transactions/{transactionId}/acknowledgment
operation_count: 21
overview: 'Orderful exposes 21 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 12 safety-critical.


  12 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Orderful
provider_slug: orderful
slug: orderful-agentic-access
source_filename: orderful-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/orderful-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    acting: 12\n    connected: 9\n  by_consequence:\n    safety-critical: 12\n    read: 9\n  human_in_the_loop_required: 12\noperations:\n- path: /v3/convert\n  method: post\n  operationId: ConversionController_convertData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/deliveries/{deliveryId}/approve\n  method:\
  \ post\n  operationId: DeliveryController_handleDeliveryApproved\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/deliveries/{deliveryId}/fail\n  method: post\n  operationId: DeliveryController_handleFailDeliveryRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /inboxes/{inboxId}/transactions\n  method: get\n  operationId: InboxController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/labels\n  method: post\n  operationId: LabelController_generate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/organizations/me\n  method: get\n  operationId: OrganizationV3Controller_getOwn\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/polling-buckets/{id}/confirm-retrieval\n  method: post\n  operationId: PollingController_confirmDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/polling-buckets/{bucketId}\n  method: get\n  operationId: PollingController_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/relationships\n  method: get\n  operationId: RelationshipController_listV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: post\n  operationId: TransactionController_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transactions/{transactionId}/deliveries/{deliveryId}\n\
  \  method: get\n  operationId: TransactionController_getDelivery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{transactionId}/deliveries/{deliveryId}/accept\n  method: post\n  operationId: TransactionController_handleDeliveryApproved\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /transactions/{transactionId}/deliveries/{deliveryId}/fail\n  method: post\n  operationId: TransactionController_handleFailDeliveryRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/transactions/{transactionId}/acknowledgment\n  method: post\n  operationId: TransactionControllerV3_acknowledgeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/transactions/{transactionId}/acknowledgment\n  method: get\n  operationId: TransactionControllerV3_getAcknowledgment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transactions/confirm-delivery\n  method: post\n  operationId: TransactionControllerV3_confirmDelivery\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/transactions\n  method: post\n  operationId: TransactionControllerV3_create\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/transactions\n  method: get\n  operationId: TransactionControllerV3_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transactions/raw\n  method: post\n  operationId: TransactionControllerV3_createRaw\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/transactions/{transactionId}\n  method: get\n  operationId: TransactionControllerV3_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transactions/{transactionId}/message\n  method: get\n  operationId: TransactionControllerV3_getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/agentic-access/orderful-agentic-access.yml
summary_line: 21 operations · 12 acting · 12 human-in-the-loop
tags:
- Company
- EDI
- Electronic Data Interchange
- Supply Chain
- B2B
- Logistics
- Retail
- Transactions
- Integration
---
