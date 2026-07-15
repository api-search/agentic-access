---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 1
api_specs:
- filename: triple-whale-openapi.yml
  format: yaml
  label: Triple Whale Summary API
  slug: triple-whale-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-openapi.yml
- filename: triple-whale-openapi.yml
  format: yaml
  label: Triple Whale Attribution API
  slug: triple-whale-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-openapi.yml
- filename: triple-whale-openapi.yml
  format: yaml
  label: Triple Whale Data-In API
  slug: triple-whale-data-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-openapi.yml
consequence_counts:
  physical: 5
  read: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Triple Whale Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /attribution/get-orders-with-journeys-v2
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data-in/bulk-orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data-in/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data-in/orders-enrichment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /data-in/pps
operation_count: 16
overview: 'Triple Whale exposes 16 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read, 10 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Triple Whale
provider_slug: triple-whale
slug: triple-whale-agentic-access
source_filename: triple-whale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/triple-whale-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 1\n    acting: 15\n  by_consequence:\n    read: 1\n    write: 10\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /users/api-keys/me\n  method: get\n  operationId: validate-your-triple-whale-api-key\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-in/ads\n  method: post\n  operationId: create-ad-record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/orders\n  method: post\n  operationId: create-order-record\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/bulk-orders\n  method: post\n  operationId: bulk-create-order-records\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/subscriptions\n\
  \  method: post\n  operationId: create-subscription-record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/products\n  method: post\n  operationId: create-product-record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/pps\n  method: post\n  operationId: create-pps-record\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/customers\n  method: post\n  operationId: create-customer-record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/orders-enrichment\n  method: post\n  operationId: enrich-orders-data\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/products-enrichment\n  method: post\n  operationId: enrich-products-data\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-in/event\n  method: post\n  operationId: enrich-pixel-with-offline-events\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orcabase/api/moby\n  method: post\n  operationId: data-out-execute-natural-language-query-moby\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orcabase/api/sql\n\
  \  method: post\n  operationId: data-out-execute-custom-sql-query\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attribution/get-orders-with-journeys-v2\n  method: post\n  operationId: get-customer-journey-attribution-data\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /summary-page/get-data\n  method: post\n  operationId: get-summary-page-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /compliance/requests/create-request\n  method: post\n  operationId: create-compliance-request\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - compliance:write\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/agentic-access/triple-whale-agentic-access.yml
summary_line: 16 operations · 15 acting
tags:
- E-commerce
- Analytics
- Attribution
- Shopify
- Pixel Tracking
- ROAS
- DTC
- Marketing
---
