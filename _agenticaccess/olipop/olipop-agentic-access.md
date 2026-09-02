---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
consequence_counts:
  physical: 3
  read: 5
  write: 5
description: ''
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: searched
name: Olipop Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Olipop exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 5 write, and 3 physical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Olipop
provider_slug: olipop
slug: olipop-agentic-access
source_filename: olipop-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://drinkolipop.com/llms.txt\nalso_from:\n- https://drinkolipop.com/agents.md\n- https://drinkolipop.com/robots.txt\n- https://ucp.dev/2026-04-08/services/shopping/mcp.openrpc.json\nnotes: >-\n  Unusually for this pipeline, the agentic-access contract here is SEARCHED rather than generated: OLIPOP\n  actually publishes agent access guidance on its own domain, in three mutually consistent places\n  (/llms.txt, /agents.md and comments at the top of /robots.txt). The operations classified below are the\n  UCP shopping tools its merchant profile declares, and the escalation rules are the provider's own stated\n  rules rather than our recommendations. Where a field is our classification rather than a published claim,\n  it is marked derived_classification.\npolicy_summary:\n  agents_welcome: true\n  agent_identity_required: true\n  identity_mechanism: UCP-Agent profile URL (meta[\"ucp-agent\"].profile)\n  read_without_enrollment:\
  \ true\n  purchase_without_human_approval: false\n  preferred_agent_path: UCP/MCP at https://drinkolipop.com/api/ucp/mcp\n  recommended_alternative: https://shop.app/SKILL.md (Shop skill / Shop Pay, for personal shopping agents)\n  prohibited:\n  - scripted checkout form fills\n  - browser automation that finalizes payment\n  - end-to-end agent flows that place an order without contemporaneous human approval\n  - screen-scraping the storefront where the UCP/MCP or Shop skill path is available (discouraged, not\n    prohibited)\n  published_verbatim_rule: >-\n    \"Checkout requires human approval. Agents must not complete payment without explicit buyer consent. If\n    you cannot get contemporaneous buyer approval at the moment of payment, install\n    https://shop.app/SKILL.md and route the purchase through Shop Pay instead.\"\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 5\n    acting: 8\n  by_consequence:\n    read: 5\n    write: 5\n    physical: 3\n  human_in_the_loop_required:\
  \ 1\n  audit_required: 8\n  idempotency_required: 3\noperations:\n- operation: search_catalog\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  audit: optional\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 3600\n- operation: lookup_catalog\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  audit: optional\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 3600\n- operation: get_product\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  audit: optional\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 3600\n- operation: get_cart\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: cart:read\n  audit: optional\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 3600\n- operation: get_checkout\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: checkout:read\n  audit:\
  \ optional\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 3600\n- operation: get_order\n  surface: ucp-mcp\n  action_class: connected\n  consequence: read\n  scope: order:read\n  audit: required\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 3600\n  note: returns buyer PII (addresses, contact details); treat as sensitive read\n- operation: create_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  audit: required\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 900\n- operation: update_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  audit: required\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 900\n- operation: cancel_cart\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  audit: required\n  human_in_the_loop: not-required\n  idempotency_key: required\n  token_ttl_max_seconds: 900\n- operation: create_checkout\n\
  \  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  audit: required\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 900\n- operation: update_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  audit: required\n  human_in_the_loop: not-required\n  token_ttl_max_seconds: 900\n  note: sets shipping address and delivery method; carries buyer PII\n- operation: cancel_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: physical\n  scope: checkout:write\n  audit: required\n  human_in_the_loop: recommended\n  idempotency_key: required\n  token_ttl_max_seconds: 300\n  note: derived_classification - cancelling a checkout is money-adjacent and irreversible from the agent's\n    side; the provider does not classify it explicitly\n- operation: complete_checkout\n  surface: ucp-mcp\n  action_class: acting\n  consequence: physical\n  scope: checkout:complete\n  audit: required\n\
  \  human_in_the_loop: required\n  purpose_required: true\n  idempotency_key: required\n  token_ttl_max_seconds: 300\n  note: PUBLISHED RULE, not a recommendation - the provider states that payment may not be completed\n    without explicit contemporaneous buyer consent\nread_only_surface:\n  description: Endpoints an agent may use with no enrollment, identity or token at all.\n  operations:\n  - 'GET /products.json'\n  - 'GET /products/{handle}.json'\n  - 'GET /collections/{handle}/products.json'\n  - 'GET /search?q={query}&type=product'\n  - 'GET /collections/all'\n  - 'GET /sitemap.xml'\n  action_class: connected\n  consequence: read\n  audience: null\n  source: https://drinkolipop.com/llms.txt\nrate_limiting:\n  scope: per IP\n  signal: HTTP 429\n  guidance: back off on 429 responses\n  published_limit: not disclosed\nbuyer_context_required:\n- context.address_country\n- context.currency\nx-evidence:\n  fetched: '2026-07-31'\n  probes:\n  - {url: 'https://drinkolipop.com/llms.txt',\
  \ http_status: 200}\n  - {url: 'https://drinkolipop.com/agents.md', http_status: 200}\n  - {url: 'https://drinkolipop.com/robots.txt', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olipop/refs/heads/main/agentic-access/olipop-agentic-access.yml
summary_line: 13 operations · 8 acting · 1 human-in-the-loop
tags:
- Beverage
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Retail
- Agent Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Shopify
- prebiotic-soda
- Functional Beverage
---
