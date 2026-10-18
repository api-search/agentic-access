---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: paack-api-systems
  format: yaml
  label: Paack API
  slug: paack-api
  spec_type: Postman
  url: https://www.postman.com/paacklogistics/paack-apis/collection/p93tvmy/paack-api-systems
- filename: paack-check-coverage-api-openapi.yml
  format: yaml
  label: Paack Check coverage API
  slug: paack-check-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/openapi/paack-check-coverage-api-openapi.yml
- filename: paack-generate-labels-api-openapi.yml
  format: yaml
  label: Paack Generate labels API
  slug: paack-generate-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/openapi/paack-generate-labels-api-openapi.yml
- filename: paack-get-access-token-api-openapi.yml
  format: yaml
  label: Paack Get access token API
  slug: paack-get-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/openapi/paack-get-access-token-api-openapi.yml
- filename: paack-manage-orders-api-openapi.yml
  format: yaml
  label: Paack Manage orders API
  slug: paack-manage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/openapi/paack-manage-orders-api-openapi.yml
- filename: paack-retrieve-delivery-proof-api-openapi.yml
  format: yaml
  label: Paack Retrieve delivery proof API
  slug: paack-retrieve-delivery-proof-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/openapi/paack-retrieve-delivery-proof-api-openapi.yml
- filename: paack-retrieve-events-history-api-openapi.yml
  format: yaml
  label: Paack Retrieve events history API
  slug: paack-retrieve-events-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/openapi/paack-retrieve-events-history-api-openapi.yml
- filename: paack-retrieve-last-event-api-openapi.yml
  format: yaml
  label: Paack Retrieve last event API
  slug: paack-retrieve-last-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/openapi/paack-retrieve-last-event-api-openapi.yml
consequence_counts:
  physical: 3
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paack Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /public/v3/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /public/v3/orders/{external_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /public/v3/orders/{external_id}
operation_count: 10
overview: 'Paack exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 2 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paack
provider_slug: paack
slug: paack-agentic-access
source_filename: paack-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/paack-api-authentication-openapi.yml, openapi/paack-coverage-api-openapi.yml,\n  openapi/paack-labeler-api-openapi.yml, openapi/paack-orders-api-openapi.yml, openapi/paack-tracking-pull-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 5\n    connected: 5\n  by_consequence:\n    write: 2\n    read: 5\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /coverage\n  method: get\n  operationId: coverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels\n  method: post\n  operationId: CreateLabelRequestPDF\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v3/orders\n  method: post\n  operationId: orders\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /public/v3/orders/{external_id}\n  method: get\n  operationId: orders-get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/v3/orders/{external_id}\n  method: put\n  operationId: orders-put\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/v3/orders/{external_id}\n  method: delete\n  operationId: orders-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /public/v3/orders/{external_id}/delivery_verifications\n  method: get\n  operationId: delivery-verifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tracking/events\n  method: get\n  operationId: list-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v3/tracking/events/latest\n  method: get\n  operationId: get-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paack/refs/heads/main/agentic-access/paack-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Company
- Logistics
- Last Mile Delivery
- Parcel Delivery
- E-Commerce
- Shipping
- Fulfillment
- Tracking
- Reverse Logistics
---
