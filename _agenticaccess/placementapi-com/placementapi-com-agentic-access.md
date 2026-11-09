---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 24
api_specs:
- filename: placementapi-com-account-api-openapi.yml
  format: yaml
  label: placementapi-com Account API
  slug: placementapi-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-account-api-openapi.yml
- filename: placementapi-com-catalogue-api-openapi.yml
  format: yaml
  label: placementapi-com Catalogue API
  slug: placementapi-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-catalogue-api-openapi.yml
- filename: placementapi-com-checkout-api-openapi.yml
  format: yaml
  label: placementapi-com Checkout API
  slug: placementapi-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-checkout-api-openapi.yml
- filename: placementapi-com-comparison-api-openapi.yml
  format: yaml
  label: placementapi-com Comparison API
  slug: placementapi-com-comparison-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-comparison-api-openapi.yml
- filename: placementapi-com-content-api-openapi.yml
  format: yaml
  label: placementapi-com Content API
  slug: placementapi-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-content-api-openapi.yml
- filename: placementapi-com-meta-api-openapi.yml
  format: yaml
  label: placementapi-com Meta API
  slug: placementapi-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-meta-api-openapi.yml
- filename: placementapi-com-orders-api-openapi.yml
  format: yaml
  label: placementapi-com Orders API
  slug: placementapi-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-orders-api-openapi.yml
- filename: placementapi-com-planning-api-openapi.yml
  format: yaml
  label: placementapi-com Planning API
  slug: placementapi-com-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-planning-api-openapi.yml
- filename: placementapi-com-research-api-openapi.yml
  format: yaml
  label: placementapi-com Research API
  slug: placementapi-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-research-api-openapi.yml
- filename: placementapi-com-search-console-api-openapi.yml
  format: yaml
  label: placementapi-com Search Console API
  slug: placementapi-com-search-console-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/placementapi-com/openapi/placementapi-com-search-console-api-openapi.yml
consequence_counts:
  physical: 10
  read: 24
  safety-critical: 2
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Placementapi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/customers/me/auto
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys/{key_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/basket
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/credits/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/observations/purchases
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{order_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{order_id}/content
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{order_id}/content/papi
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/standing_orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/standing_orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/standing_orders/{id}
operation_count: 49
overview: 'placementapi-com exposes 49 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 13 write, 10 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: placementapi-com
provider_slug: placementapi-com
slug: placementapi-com-agentic-access
source_filename: placementapi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/placementapi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 24\n    acting: 25\n  by_consequence:\n    read: 24\n    write: 13\n    physical: 10\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /v1\n  method: get\n  operationId: service_banner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/schema\n\
  \  method: get\n  operationId: field_semantics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offers\n  method: get\n  operationId: search_placements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sites/{domain}\n  method: get\n  operationId: compare_domain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market\n  method: get\n  operationId: market_prices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/taste\n  method: get\n  operationId: market_taste\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quote\n  method: post\n  operationId: plan_links\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes/{quote_id}\n  method: get\n  operationId: get_quote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/campaigns\n  method: get\n  operationId: campaign_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/targets/profile\n  method: get\n  operationId: target_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/targets/gap\n  method: post\n  operationId: gap_map\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keywords/winners\n  method: get\n  operationId: keyword_winners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders\n  method: post\n  operationId: place_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/orders\n  method: get\n  operationId: list_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{order_id}/cancel\n  method: post\n  operationId: cancel_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{order_id}/outcome\n  method: get\n  operationId: order_outcome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{order_id}/content\n  method: post\n  operationId: submit_content\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders/{order_id}/content\n  method: get\n  operationId: get_order_content\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{order_id}/content/papi\n  method: post\n  operationId: write_it_for_me\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits\n  method: get\n  operationId: check_balance\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/checkout\n  method: post\n  operationId: create_topup_checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits/settings\n  method: get\n  operationId: get_spend_settings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/settings\n  method: patch\n  operationId: update_spend_settings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: get\n  operationId: list_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: create_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{key_id}\n  method: patch\n  operationId: rename_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/keys/{key_id}\n  method: delete\n  operationId: revoke_key\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/customers/me\n  method: get\n  operationId: get_account_profile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/me\n  method: patch\n  operationId: update_account_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/me/email\n\
  \  method: post\n  operationId: request_email_change\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/me/email/confirm\n  method: post\n  operationId: confirm_email_change\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/logout\n  method: post\n  operationId: logout\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/customers/me/brief\n  method: get\n  operationId: get_weekly_brief\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/me/brief\n  method: patch\n  operationId: update_weekly_brief\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/me/auto\n  method: get\n  operationId: get_auto_placement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/me/auto\n  method: post\n  operationId: set_auto_placement\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/standing_orders\n  method: get\n  operationId: standing_orders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/standing_orders\n  method: post\n  operationId: create_standing_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/standing_orders/{id}\n  method: patch\n  operationId: update_standing_order\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/standing_orders/{id}\n  method: delete\n  operationId: delete_standing_order\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/basket\n  method: post\n  operationId: checkout_basket\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/basket/{basket_id}\n  method: get\n  operationId: checkout_basket_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/observations/purchases\n  method: post\n  operationId: report_purchases\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/perch/compare\n  method: post\n  operationId: perch_compare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/baskets/compare\n  method: post\n  operationId: compare_basket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gsc/properties\n  method: get\n  operationId: gsc_properties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gsc/properties\n  method: patch\n  operationId: gsc_select_properties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gsc/daily\n  method: get\n  operationId: gsc_daily_rows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/placementapi-com/agentic-access/placementapi-com-agentic-access.yml
summary_line: 49 operations · 25 acting · 2 human-in-the-loop
tags:
- Company
- Artificial Intelligence
- SEO
- Marketing
- Backlinks
- Automation
- Technology
---
