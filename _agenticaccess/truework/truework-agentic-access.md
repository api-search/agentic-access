---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: truework-verifications-orders-openapi.yml
  format: yaml
  label: Truework Verifications API
  slug: truework-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-verifications-orders-openapi.yml
- filename: truework-beta-openapi.yml
  format: yaml
  label: Truework Qualifications API (Beta)
  slug: truework-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-beta-openapi.yml
- filename: truework-beta-openapi.yml
  format: yaml
  label: Truework Tenant Properties API (Beta)
  slug: truework-tenant-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-beta-openapi.yml
- filename: truework-webhooks-openapi.yml
  format: yaml
  label: Truework Webhooks
  slug: truework-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/openapi/truework-webhooks-openapi.yml
consequence_counts:
  physical: 5
  read: 8
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Truework Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/employer-search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/reverification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/target-employer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/truework-direct
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /orders/{order_id}/cancel
operation_count: 16
overview: 'Truework exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 3 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Truework
provider_slug: truework
slug: truework-agentic-access
source_filename: truework-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/truework-beta-openapi.yml, openapi/truework-verifications-orders-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 8\n    connected: 8\n  by_consequence:\n    write: 3\n    read: 8\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /qualification-checks\n  method: post\n  operationId: create-new-qualification-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /qualification-checks/{qualification_check_result_id}\n\
  \  method: get\n  operationId: get-one-qualification-check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /qualification-check-sets\n  method: get\n  operationId: get-all-qualification-check-sets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenant-properties\n  method: post\n  operationId: create-new-tenant-property\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tenant-properties\n  method: get\n  operationId: get-all-tenant-properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /tenant-properties/{tenant_property_id}\n  method: get\n  operationId: get-one-tenant-property\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenant-properties/{tenant_property_id}\n  method: put\n  operationId: update-one-tenant-property\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/target-employer\n  method: post\n  operationId: create-new-target-employer-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/employer-search\n  method: post\n  operationId: create-new-order-employer-search-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/truework-direct\n  method: post\n  operationId: create-new-truework-direct-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/{order_id}\n\
  \  method: get\n  operationId: get-one-order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: get\n  operationId: get-all-orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/cancel\n  method: put\n  operationId: cancel-an-order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/{verification_report_id}\n  method: get\n  operationId: get-report-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/{order_id}/events\n  method: get\n  operationId: get-order-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders/reverification\n  method: post\n  operationId: reverify-a-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truework/refs/heads/main/agentic-access/truework-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Verifications
- Income Verification
- Employment Verification
- VOIE
- Mortgage
- Lending
- Credit Unions
- Identity
- KYC
- Fintech
---
