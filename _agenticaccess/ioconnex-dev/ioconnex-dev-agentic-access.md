---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 16
api_specs:
- filename: ioconnex-dev-affiliate-api-openapi.yml
  format: yaml
  label: ioconnex-dev Affiliate API
  slug: ioconnex-dev-affiliate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-affiliate-api-openapi.yml
- filename: ioconnex-dev-billing-api-openapi.yml
  format: yaml
  label: ioconnex-dev Billing API
  slug: ioconnex-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-billing-api-openapi.yml
- filename: ioconnex-dev-convert-api-openapi.yml
  format: yaml
  label: ioconnex-dev Convert API
  slug: ioconnex-dev-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-convert-api-openapi.yml
- filename: ioconnex-dev-fetch-api-openapi.yml
  format: yaml
  label: ioconnex-dev Fetch API
  slug: ioconnex-dev-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-fetch-api-openapi.yml
- filename: ioconnex-dev-health-api-openapi.yml
  format: yaml
  label: ioconnex-dev Health API
  slug: ioconnex-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-health-api-openapi.yml
- filename: ioconnex-dev-paid-api-openapi.yml
  format: yaml
  label: ioconnex-dev Paid API
  slug: ioconnex-dev-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-paid-api-openapi.yml
- filename: ioconnex-dev-price-api-openapi.yml
  format: yaml
  label: ioconnex-dev Price API
  slug: ioconnex-dev-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-price-api-openapi.yml
- filename: ioconnex-dev-search-api-openapi.yml
  format: yaml
  label: ioconnex-dev Search API
  slug: ioconnex-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ioconnex-dev/openapi/ioconnex-dev-search-api-openapi.yml
consequence_counts:
  physical: 3
  read: 16
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ioconnex Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /billing/checkout
operation_count: 30
overview: 'ioconnex-dev exposes 30 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 11 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ioconnex-dev
provider_slug: ioconnex-dev
slug: ioconnex-dev-agentic-access
source_filename: ioconnex-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/convert-openapi.json, openapi/prices-openapi.json, openapi/search-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    connected: 16\n    acting: 14\n  by_consequence:\n    read: 16\n    write: 11\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /convert/pdf\n  method: post\n  operationId: convert_pdf_convert_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paid/convert/pdf\n  method: post\n  operationId: convert_pdf_paid_convert_pdf_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /convert/ocr\n  method: post\n  operationId: convert_ocr_convert_ocr_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /convert/spreadsheet\n  method: post\n  operationId: convert_spreadsheet_convert_spreadsheet_post\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /convert/url\n  method: post\n  operationId: convert_url_convert_url_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/checkout\n  method: post\n  operationId: billing_checkout_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /billing/stripe-webhook\n  method: post\n  operationId: stripe_webhook_billing_stripe_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/key\n  method: get\n  operationId: billing_key_billing_key_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage\n  method: get\n  operationId: billing_usage_billing_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/status\n  method: get\n  operationId: billing_status_billing_status_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/checkout\n  method: post\n  operationId: billing_checkout_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/stripe-webhook\n  method: post\n  operationId: stripe_webhook_billing_stripe_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/key\n  method: get\n  operationId: billing_key_billing_key_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/status\n  method: get\n  operationId: billing_status_billing_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage\n  method: get\n  operationId: billing_usage_billing_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/stats\n  method: get\n  operationId: billing_stats_billing_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price\n  method: post\n  operationId: price_price_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paid/price\n  method: post\n  operationId: price_paid_price_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /affiliate\n  method: post\n  operationId: affiliate_affiliate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/checkout\n  method: post\n  operationId: checkout_billing_checkout_post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/stripe-webhook\n  method: post\n  operationId: stripe_webhook_billing_stripe_webhook_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /billing/key\n  method: get\n  operationId: get_key_billing_key_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/usage\n  method: get\n  operationId: usage_billing_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /billing/status\n  method: get\n  operationId: billing_status_billing_status_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: search_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/search\n  method: post\n  operationId: search_paid_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fetch\n  method: post\n  operationId: fetch_fetch_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ioconnex-dev/agentic-access/ioconnex-dev-agentic-access.yml
summary_line: 30 operations · 14 acting
tags:
- Company
- Artificial Intelligence
- MCP
- Search
- Document Conversion
- Price-Tracking
---
