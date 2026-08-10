---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 4
  read: 4
consequence_counts:
  physical: 3
  read: 8
  write: 6
description: ''
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Tecovas Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Tecovas exposes 17 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 6 write, and 3 physical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tecovas
provider_slug: tecovas
slug: tecovas-agentic-access
source_filename: tecovas-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: mcp/tecovas-ucp-tools-list.json + well-known/tecovas-api-catalog.json + https://checkout.tecovas.com/agents.md\nnote: >-\n  A recommended x-agentic-access execution contract per operation, classified with the standard\n  pipeline heuristics (read/connected for GET, acting/write for mutations, consequence raised to\n  physical on payment and order operations). This is a governance starting point, not a Tecovas\n  claim. It is unusual in one respect: Tecovas already publishes a human-in-the-loop invariant of\n  its own — both agents.md documents forbid completing checkout or payment without explicit,\n  contemporaneous buyer approval — so the human_in_the_loop values on the checkout tools below\n  are the provider's stated policy, not our inference. `audience` is left null to bind per\n  deployment.\nsummary:\n  operations: 17\n  by_action_class: {connected: 4, read: 4, acting: 9}\n  by_consequence: {read: 8, write: 6, physical:\
  \ 3}\n  human_in_the_loop_required: 3\n  provider_stated_human_approval: true\n  provider_source: https://checkout.tecovas.com/agents.md\noperations:\n- id: GET /api/productdetail/:slug\n  surface: storefront-json\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n- id: GET /api/collection\n  surface: storefront-json\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n- id: GET /api/collection-products\n  surface: storefront-json\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n  note: 'Rate-limit sensitive — the provider asks agents to cap responses with ?limit=.'\n- id: GET /api/search-settings\n  surface: storefront-json\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n\
  - id: search_catalog\n  surface: ucp-mcp\n  action_class: read\n  consequence: read\n  scope: catalog:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n- id: lookup_catalog\n  surface: ucp-mcp\n  action_class: read\n  consequence: read\n  scope: catalog:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n- id: get_product\n  surface: ucp-mcp\n  action_class: read\n  consequence: read\n  scope: catalog:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n- id: get_cart\n  surface: ucp-mcp\n  action_class: read\n  consequence: read\n  scope: cart:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n- id: create_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token_ttl_max: 900\n  audience: null\n  audit: required\n- id: update_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token_ttl_max: 900\n  audience: null\n  audit: required\n- id: cancel_cart\n\
  \  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token_ttl_max: 900\n  audience: null\n  audit: required\n- id: create_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  token_ttl_max: 900\n  audience: null\n  audit: required\n- id: get_checkout\n  surface: ucp-mcp\n  action_class: read\n  consequence: read\n  scope: checkout:read\n  token_ttl_max: 3600\n  audience: null\n  audit: optional\n- id: update_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: physical\n  scope: checkout:write\n  token_ttl_max: 300\n  audience: null\n  audit: required\n  token_exchange: true\n  purpose_required: true\n  note: Carries shipping address, delivery method and payment instrument selection.\n- id: complete_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: physical\n  scope: checkout:complete\n  token_ttl_max: 300\n  audience: null\n  audit: required\n  token_exchange: true\n\
  \  purpose_required: true\n  human_in_the_loop: required\n  human_in_the_loop_source: https://checkout.tecovas.com/agents.md\n  note: >-\n    Finalizes payment and places a real order for physical goods. The provider explicitly\n    forbids completing this without contemporaneous buyer approval.\n- id: cancel_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: physical\n  scope: checkout:write\n  token_ttl_max: 300\n  audience: null\n  audit: required\n  human_in_the_loop: required\n  human_in_the_loop_source: https://checkout.tecovas.com/agents.md\n  note: Destructive against a buyer-owned checkout.\n- id: get_order\n  surface: ucp-mcp\n  action_class: read\n  consequence: read\n  scope: customer-account-api:full\n  token_ttl_max: 3600\n  audience: null\n  audit: required\n  note: >-\n    Returns buyer PII (addresses, purchase history). Requires an authenticated Shopify customer\n    account token; the human_in_the_loop decision belongs to the consent flow, not this call.\n\
  prohibited_by_provider:\n  source: https://www.tecovas.com/agents.md\n  rules:\n  - Do not complete checkout, payment or order placement automatically.\n  - No scripted form fills or browser automation that finalize payment without explicit human approval.\n  - 'Do not access robots.txt-disallowed paths: /account, /admin, /cart, /carts, /checkout, /checkouts/, /orders/*.'\n  - Honor Crawl-delay directives and back off on 429.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - {url: 'https://checkout.tecovas.com/api/ucp/mcp', status: 200, note: 'POST tools/list — 13 tools classified'}\n  - {url: 'https://checkout.tecovas.com/agents.md', status: 200}\n  - {url: 'https://www.tecovas.com/agents.md', status: 200}\n  - {url: 'https://www.tecovas.com/.well-known/api-catalog', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecovas/refs/heads/main/agentic-access/tecovas-agentic-access.yml
summary_line: 17 operations · 9 acting · 3 human-in-the-loop
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Footwear
- Direct to Consumer
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- Product Catalog
---
