---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 8
api_specs:
- filename: lengow-channel-execution-openapi.yml
  format: yaml
  label: Lengow Channel Execution API
  slug: lengow-channel-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/openapi/lengow-channel-execution-openapi.yml
consequence_counts:
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lengow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Lengow exposes 14 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lengow
provider_slug: lengow
slug: lengow-agentic-access
source_filename: lengow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: generated\nsource: openapi/lengow-channel-execution-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 6\n    connected: 8\n  by_consequence:\n    write: 6\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /access/get_token\n  method: post\n  operationId: Get Authentication Token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: Get Current Session\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rate-limits\n  method: get\n  operationId: Get Rate Limits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/catalogues\n  method: get\n  operationId: list_catalogues_public_catalogues_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/catalogues/{catalogue_id}\n  method: get\n  operationId: get_catalogue_public_catalogues__catalogue_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/catalogues/{catalogue_id}/attributes\n  method: get\n  operationId: list_attributes_public_catalogues__catalogue_id__attributes_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/catalogues/{catalogue_id}/products\n  method: delete\n  operationId: delete_products_public_catalogues__catalogue_id__products_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/catalogues/{catalogue_id}/products\n  method: get\n  operationId: list_products_public_catalogues__catalogue_id__products_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/catalogues/{catalogue_id}/products\n  method: patch\n  operationId: update_products_public_catalogues__catalogue_id__products_patch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/catalogues/{catalogue_id}/products\n  method: post\n  operationId: upsert_products_public_catalogues__catalogue_id__products_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/catalogues/{catalogue_id}/products/{product_id_value}\n  method: delete\n  operationId: delete_product_public_catalogues__catalogue_id__products__product_id_value__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1.0/catalogues/{catalogue_id}/products/{product_id_value}\n  method: get\n  operationId: get_product_public_catalogues__catalogue_id__products__product_id_value__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1.0/catalogues/{catalogue_id}/products/{product_id_value}\n  method: patch\n  operationId: update_product_public_catalogues__catalogue_id__products__product_id_value__patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3.0/report/export\n  method: get\n  operationId: Get product reports\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lengow/refs/heads/main/agentic-access/lengow-agentic-access.yml
summary_line: 14 operations · 6 acting
tags:
- Company
- SaaS
- E-Commerce
- Marketplaces
- Product Feeds
- Retail
- Advertising
- Order Management
- Price Intelligence
- France
---
