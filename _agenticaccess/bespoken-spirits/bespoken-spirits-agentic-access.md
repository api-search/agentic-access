---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
consequence_counts:
  physical: 1
  read: 10
  write: 7
description: ''
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Bespoken Spirits Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Bespoken Spirits exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 7 write, and 1 physical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bespoken Spirits
provider_slug: bespoken-spirits
slug: bespoken-spirits-agentic-access
source_filename: bespoken-spirits-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: generated\nsource: mcp/bespoken-spirits-ucp-mcp-tools.json\naudience: null\nnotes: >-\n  A recommended x-agentic-access execution contract per operation, classified from the\n  live MCP tool set rather than from an OpenAPI (Bespoken Spirits publishes none). This\n  is a governance starting point produced by API Evangelist, not a provider claim.\n  Two of the controls below are NOT recommendations but observed provider behaviour and\n  are marked source: provider — the mandatory human approval on complete_checkout, and\n  the idempotency key it requires. Both are stated on the company's own surface.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 10\n    acting: 8\n  by_consequence:\n    read: 10\n    write: 7\n    physical: 1\n  human_in_the_loop_required: 1\n  audit_required: 8\nsurfaces:\n- name: ucp-mcp\n  url: https://bespokenspirits.com/api/ucp/mcp\n  operations: 13\n- name: storefront-mcp\n  url: https://bespokenspirits.com/api/mcp\n\
  \  operations: 5\noperations:\n- operation: search_catalog\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: lookup_catalog\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: get_product\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: get_cart\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: cart:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: get_checkout\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: checkout:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: get_order\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: order:read\n  token_ttl_seconds: 3600\n  audit: optional\n\
  - operation: create_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token_ttl_seconds: 900\n  audit: required\n- operation: update_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token_ttl_seconds: 900\n  audit: required\n- operation: cancel_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token_ttl_seconds: 900\n  audit: required\n- operation: create_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  token_ttl_seconds: 900\n  audit: required\n  note: >-\n    Recommend an idempotency key here even though the provider does not require one —\n    a blind retry creates a duplicate checkout.\n- operation: update_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  token_ttl_seconds: 900\n  audit: required\n- operation: cancel_checkout\n  surface: ucp-mcp\n\
  \  action_class: acting\n  consequence: write\n  scope: checkout:write\n  token_ttl_seconds: 900\n  audit: required\n- operation: complete_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: physical\n  scope: checkout:complete\n  token_ttl_seconds: 300\n  token_exchange: required\n  purpose_required: true\n  human_in_the_loop: required\n  human_in_the_loop_source: provider\n  audit: required\n  idempotency_key: meta.idempotency-key\n  idempotency_source: provider\n  note: >-\n    Moves money and ships a regulated product (beverage alcohol). The provider itself\n    mandates contemporaneous buyer approval in llms.txt, agents.md and robots.txt, and\n    requires meta.idempotency-key on the call. Age and jurisdiction eligibility are\n    carried in context.eligibility.\n- operation: search_catalog\n  surface: storefront-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: get_product_details\n\
  \  surface: storefront-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: search_shop_policies_and_faqs\n  surface: storefront-mcp\n  action_class: connected\n  consequence: read\n  scope: content:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: get_cart\n  surface: storefront-mcp\n  action_class: connected\n  consequence: read\n  scope: cart:read\n  token_ttl_seconds: 3600\n  audit: optional\n- operation: update_cart\n  surface: storefront-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token_ttl_seconds: 900\n  audit: required\nx-evidence:\n  fetched: '2026-08-07'\n  probes:\n  - url: https://bespokenspirits.com/api/ucp/mcp\n    method: POST tools/list\n    http_status: 200\n  - url: https://bespokenspirits.com/api/mcp\n    method: POST tools/list\n    http_status: 200\n  - url: https://bespokenspirits.com/robots.txt\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bespoken-spirits/refs/heads/main/agentic-access/bespoken-spirits-agentic-access.yml
summary_line: 18 operations · 8 acting · 1 human-in-the-loop
tags:
- Company
- Spirits
- Beverage Alcohol
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Retail
- Manufacturing
---
