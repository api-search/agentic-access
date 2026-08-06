---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Everytable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Everytable exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Everytable
provider_slug: everytable
slug: everytable-agentic-access
source_filename: everytable-agentic-access.yml
source_heading: Agentic Access
source_url: https://everytable.com/agents.md
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://everytable.com/agents.md\nsources:\n- https://everytable.com/agents.md\n- https://everytable.com/llms.txt\n- https://everytable.com/robots.txt\n- https://everytable.com/.well-known/ucp\nnote: Everytable publishes an explicit, machine-readable agent access policy on its\n  own host. This artifact records that published policy verbatim in structure; it is\n  not a generated recommendation derived from an OpenAPI.\nsummary:\n  publishes_agent_policy: true\n  policy_surfaces:\n  - /agents.md\n  - /llms.txt\n  - /robots.txt\n  - /.well-known/ucp\n  - /sitemap_agentic_discovery.xml\n  preferred_agent_transport: mcp\n  human_in_the_loop_required_for:\n  - payment\n  - checkout completion\n  - order placement\n  crawling_permitted: true\n  scripted_checkout_permitted: false\npolicy:\n  crawl:\n    stance: allow\n    detail: 'robots.txt allows public product, collection, page, blog, policy, cart\n      and localized HTML. Disallowed:\
  \ /admin, /cart/, /checkout, /checkouts/, /orders,\n      /account, /services, /sf_*, /cart.js, /recommendations/products, and filter/sort\n      crawl traps.'\n    source: https://everytable.com/robots.txt\n  transact:\n    stance: allow-with-human-approval\n    detail: Agents transacting on a buyer's behalf must use the UCP/MCP endpoint or\n      the Shopify shopping skill; both require buyer approval before payment.\n    source: https://everytable.com/agents.md\n  prohibited:\n  - id: automated-checkout\n    rule: Do NOT complete checkout, payment, or order placement automatically — no\n      scripted form fills, browser automation, or end-to-end agent flows that finalize\n      payment without an explicit, contemporaneous human approval step.\n    source: https://everytable.com/robots.txt\n  - id: storefront-scripting\n    rule: Agents should prefer the Shop skill / UCP-MCP over screen-scraping or scripting\n      the storefront directly.\n    source: https://everytable.com/agents.md\n\
  \  - id: ajax-surfaces\n    rule: AJAX surfaces (/cart.js, /recommendations/products) are disallowed to crawlers;\n      agents should use UCP/MCP instead.\n    source: https://everytable.com/robots.txt\noperations:\n- id: read_catalog\n  surface: https://everytable.com/products/{handle}.json\n  action_class: connected\n  consequence: read\n  authentication: none\n  human_in_the_loop: not-required\n  audit: not-required\n  source: https://everytable.com/llms.txt\n- id: search_catalog\n  surface: mcp://everytable.com/api/ucp/mcp#search_catalog\n  action_class: connected\n  consequence: read\n  authentication: ucp-agent-profile\n  human_in_the_loop: not-required\n  audit: not-required\n- id: create_cart\n  surface: mcp://everytable.com/api/ucp/mcp#create_cart\n  action_class: acting\n  consequence: write\n  authentication: ucp-agent-profile\n  human_in_the_loop: not-required\n  audit: recommended\n- id: create_checkout\n  surface: mcp://everytable.com/api/ucp/mcp#create_checkout\n  action_class:\
  \ acting\n  consequence: write\n  authentication: ucp-agent-profile\n  human_in_the_loop: not-required\n  audit: required\n- id: update_checkout\n  surface: mcp://everytable.com/api/ucp/mcp#update_checkout\n  action_class: acting\n  consequence: write\n  authentication: ucp-agent-profile\n  human_in_the_loop: not-required\n  audit: required\n- id: complete_checkout\n  surface: mcp://everytable.com/api/ucp/mcp#complete_checkout\n  action_class: acting\n  consequence: physical\n  authentication: ucp-agent-profile + buyer-approved payment handler\n  human_in_the_loop: required\n  audit: required\n  rule_source: https://everytable.com/robots.txt\n  note: Provider-stated, not inferred — Everytable requires explicit contemporaneous\n    human approval at the moment of payment.\npayment_handlers:\n- shop_pay\n- shopify.card\n- gpay\nrate_limits:\n  stated: The MCP endpoint is rate-limited per IP. Back off on 429 responses.\n  source: https://everytable.com/llms.txt\nbuyer_context:\n  recommended_fields:\n\
  \  - context.address_country\n  - context.currency\n  source: https://everytable.com/llms.txt\nx-evidence:\n  fetched: '2026-08-04'\n  urls:\n  - url: https://everytable.com/agents.md\n    http_status: 200\n    content_type: text/markdown\n  - url: https://everytable.com/llms.txt\n    http_status: 200\n    content_type: text/markdown\n  - url: https://everytable.com/robots.txt\n    http_status: 200\n    content_type: text/plain\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everytable/refs/heads/main/agentic-access/everytable-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Food
- Restaurants
- Meal Delivery
- Ecommerce
- Agentic Commerce
- Shopify
- Social Enterprise
- Nutrition
- Subscriptions
---
