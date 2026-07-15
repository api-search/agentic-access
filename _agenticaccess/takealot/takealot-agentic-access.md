---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 11
api_specs:
- filename: takealot-seller-openapi.yml
  format: yaml
  label: Takealot Seller API
  slug: seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-seller-openapi.yml
consequence_counts:
  read: 11
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Takealot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Takealot exposes 16 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Takealot
provider_slug: takealot
slug: takealot-agentic-access
source_filename: takealot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/takealot-seller-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 11\n    acting: 5\n  by_consequence:\n    read: 11\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/offers\n  method: get\n  operationId: get_offers_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/offers/count\n  method: get\n  operationId: get_offers_count_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/offers/offer/{identifier}\n\
  \  method: get\n  operationId: get_offer_by_identifier_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/offers/offer/{identifier}\n  method: patch\n  operationId: update_offer_by_identifier_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/offers/offer/{identifier}\n  method: post\n  operationId: create_offer_by_identifier_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/offers/offer\n  method: get\n\
  \  operationId: get_offer_by_identifier_query_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/offers/offer\n  method: patch\n  operationId: update_offer_by_identifier_query_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/offers/offer\n  method: post\n  operationId: create_offer_by_identifier_query_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/offers/batch\n  method: post\n  operationId: create_batch_v2\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/offers/batch/{batch_id}\n  method: get\n  operationId: get_batch_v2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{version}/offers/stock_counts\n  method: get\n  operationId: get_total_and_unbalanced_stock_at_tal_counts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{version}/offers/stock_health_stats\n  method: get\n  operationId: get_stock_health_stats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /{version}/sales\n  method: get\n  operationId: view_sales\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{version}/sales/summary\n  method: get\n  operationId: get_sales_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{version}/sales/orders\n  method: get\n  operationId: get_sales_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{version}/sales/orders/{order_id}/customer_invoices\n  method: get\n  operationId: get_sales_order_customer_invoices_credit_notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/agentic-access/takealot-agentic-access.yml
summary_line: 16 operations · 5 acting
tags:
- Commerce
- E-Commerce
- Marketplace
- Retail
- Marketplace Sellers
- Offers
- Orders
- Sales
- Stock Management
- Fulfilment
- Logistics
- Food Delivery
- South Africa
- Africa
- Naspers
- Prosus
---
