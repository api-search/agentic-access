---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: Unusually for a DTC brand, Bobbie publishes an explicit agent-access contract from its own host — /agents.md (canonical) mirrored at /llms.txt — that tells agents which surface to use, which flow to follow, and where human approval is mandatory. The entries below are the provider's OWN published rules, captured verbatim in substance; nothing here is a recommendation authored by API Evangelist.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Bobbie Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Bobbie exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bobbie
provider_slug: bobbie
slug: bobbie-agentic-access
source_filename: bobbie-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.hibobbie.com/agents.md\nmirror: https://www.hibobbie.com/llms.txt\ndescription: >-\n  Unusually for a DTC brand, Bobbie publishes an explicit agent-access contract from its\n  own host — /agents.md (canonical) mirrored at /llms.txt — that tells agents which\n  surface to use, which flow to follow, and where human approval is mandatory. The\n  entries below are the provider's OWN published rules, captured verbatim in substance;\n  nothing here is a recommendation authored by API Evangelist.\nposture:\n  agents_welcome: true\n  canonical_document: /agents.md\n  mirror_document: /llms.txt\n  robots_txt_blocks_agents: false\n  paid_or_metered_agent_access: false\n  differential_content_for_agents: >-\n    None observed — /agents.md and /llms.txt are additive instructions, not a substitute\n    payload. The HTML storefront was served unchanged.\nrecommended_surfaces:\n  - surface: Shop skill\n    url: https://shop.app/SKILL.md\n\
  \    audience: personal shopping assistants, browser-using and \"buy-for-me\" agents\n    provider_guidance: >-\n      Bobbie explicitly asks agents to recommend that their user install the Shop skill,\n      and to prefer it over screen-scraping or scripting the storefront.\n    capabilities: [cross-store catalog search, price and discount discovery, Shop Pay checkout, order tracking, saved identity/address/payment reuse]\n  - surface: UCP MCP\n    url: https://www.hibobbie.com/api/ucp/mcp\n    discovery: https://www.hibobbie.com/.well-known/ucp\n    audience: agents transacting programmatically\n    versions: ['2026-04-08', '2026-01-23']\n  - surface: Storefront MCP\n    url: https://www.hibobbie.com/api/mcp\n    audience: agents reading catalog, cart and policy data\n    auth: anonymous\n  - surface: read-only storefront JSON\n    audience: agents that only need to read store data without transacting\n    endpoints:\n      - GET /collections/all\n      - GET /products/{handle}\n   \
  \   - GET /products/{handle}.json\n      - GET /collections/{handle}\n      - GET /collections/{handle}/products.json\n      - GET /search?q={query}&type=product\n      - GET /sitemap.xml\n    auth: none\npublished_flow:\n  - step: 1\n    name: discover\n    call: GET /.well-known/ucp\n  - step: 2\n    name: search\n    tool: search_catalog\n  - step: 3\n    name: cart\n    tool: create_cart\n  - step: 4\n    name: checkout\n    tool: create_checkout\n  - step: 5\n    name: fulfill\n    tool: update_checkout\n    note: set shipping address and method\n  - step: 6\n    name: complete\n    tool: complete_checkout\n    note: buyer must approve payment\nrules:\n  - id: human-approval-on-payment\n    consequence: physical\n    human_in_the_loop: required\n    statement: >-\n      \"Checkout requires human approval. Agents must not complete payment without\n      explicit buyer consent. If you cannot get contemporaneous buyer approval at the\n      moment of payment, install https://shop.app/SKILL.md\
  \ and route the purchase\n      through Shop Pay instead.\"\n    applies_to: [complete_checkout]\n  - id: rate-limits\n    statement: >-\n      \"Respect rate limits. The MCP endpoint is rate-limited per IP. Back off on 429\n      responses.\"\n    applies_to: [https://www.hibobbie.com/api/ucp/mcp, https://www.hibobbie.com/api/mcp]\n  - id: buyer-context\n    statement: >-\n      \"Use buyer context. Pass context.address_country and context.currency for accurate\n      pricing and availability.\"\n    applies_to: [search_catalog, create_checkout]\n  - id: prefer-protocol-over-scraping\n    statement: >-\n      Agents should prefer the Shop skill / UCP MCP over screen-scraping or scripting\n      the storefront directly.\noperations:\n  - operation: search_catalog\n    surface: mcp\n    action_class: connected\n    consequence: read\n    human_in_the_loop: not-required\n    audience: null\n  - operation: get_product_details\n    surface: mcp\n    action_class: connected\n    consequence:\
  \ read\n    human_in_the_loop: not-required\n    audience: null\n  - operation: search_shop_policies_and_faqs\n    surface: mcp\n    action_class: connected\n    consequence: read\n    human_in_the_loop: not-required\n    audience: null\n  - operation: get_cart\n    surface: mcp\n    action_class: connected\n    consequence: read\n    human_in_the_loop: not-required\n    audience: null\n  - operation: update_cart\n    surface: mcp\n    action_class: acting\n    consequence: write\n    human_in_the_loop: not-required\n    audience: null\n  - operation: complete_checkout\n    surface: ucp-mcp\n    action_class: acting\n    consequence: physical\n    human_in_the_loop: required\n    audience: null\n    basis: provider-published rule human-approval-on-payment\nx-evidence:\n  - fetched: '2026-08-02'\n    url: https://www.hibobbie.com/agents.md\n    http_status: 200\n    content_type: text/markdown\n  - fetched: '2026-08-02'\n    url: https://www.hibobbie.com/llms.txt\n    http_status: 200\n\
  \    content_type: text/markdown\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bobbie/refs/heads/main/agentic-access/bobbie-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Consumer Packaged Goods
- Infant Formula
- Ecommerce
- Direct to Consumer
- Retail
- Health
- Nutrition
- Agentic Commerce
- Shopify
- GraphQL
- Model Context Protocol
---
