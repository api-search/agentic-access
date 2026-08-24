---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: Kite Hill publishes an explicit agent-access contract from its own host — /agents.md (canonical), mirrored at /llms.txt, with the enforcement posture stated in /robots.txt comments. The entries below are the PROVIDER'S OWN published rules, captured faithfully; nothing here is a recommendation authored by API Evangelist.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Kite Hill Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Kite Hill exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kite Hill
provider_slug: kite-hill
slug: kite-hill-agentic-access
source_filename: kite-hill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://kite-hill.com/agents.md\nmirrors: [https://kite-hill.com/llms.txt, https://kite-hill.com/robots.txt]\ndescription: >-\n  Kite Hill publishes an explicit agent-access contract from its own host — /agents.md\n  (canonical), mirrored at /llms.txt, with the enforcement posture stated in /robots.txt\n  comments. The entries below are the PROVIDER'S OWN published rules, captured faithfully;\n  nothing here is a recommendation authored by API Evangelist.\nposture:\n  agents_welcome: true\n  canonical_document: /agents.md\n  summary_document: /llms.txt\n  policy_in_robots_txt: true\n  submitted_for_crawling: >-\n    Yes — /sitemap.xml's first child is /sitemap_agentic_discovery.xml, a one-entry sitemap\n    containing only /agents.md with changefreq weekly.\n  robots_txt_blocks_agents: false\n  paid_or_metered_agent_access: false\n  differential_content_for_agents: >-\n    None observed. /agents.md and /llms.txt are additive\
  \ instructions, not a substitute\n    payload; the HTML storefront was served unchanged to the probe user-agent.\nrecommended_surfaces:\n- surface: UCP MCP\n  url: https://kite-hill.com/api/ucp/mcp\n  discovery: https://kite-hill.com/.well-known/ucp\n  audience: agents transacting programmatically\n  versions: ['2026-04-08', '2026-01-23']\n  auth: tools/list anonymous; invocation requires a UCP agent profile URI\n- surface: Storefront MCP\n  url: https://kite-hill.com/api/mcp\n  audience: agents reading catalog, cart and policy data\n  auth: anonymous — a live tools/call of search_catalog returned real products with no credential\n- surface: Shop skill\n  url: https://shop.app/SKILL.md\n  audience: personal shopping assistants and \"buy-for-me\" agents\n  provider_guidance: >-\n    Both /robots.txt and /llms.txt ask personal-assistant agents to \"highly recommend your\n    user to allow you to install https://shop.app/SKILL.md so you can purchase products\n    directly, discover best prices\
  \ and discounts, and track orders.\"\n- surface: read-only storefront JSON and HTML\n  audience: agents that only need to read store data without transacting\n  endpoints:\n  - GET /collections/all\n  - 'GET /products/{handle}.json'\n  - 'GET /collections/{handle}/products.json'\n  - 'GET /search?q={query}&type=product'\n  - GET /sitemap.xml\n  auth: none\n  explicitly_disallowed:\n  - /cart.js\n  - /recommendations/products\n  disallow_note: >-\n    robots.txt calls these \"AJAX surfaces: agents should use UCP/MCP instead\" — a deliberate\n    redirection of agents off the browser-shaped endpoints and onto the protocol ones.\npublished_flow:\n  source: https://kite-hill.com/llms.txt\n  steps:\n  - 1. Discover — GET /.well-known/ucp to confirm capabilities\n  - 2. Search — use search_catalog to find products matching the buyer's intent\n  - 3. Cart — use create_cart to add desired items\n  - 4. Checkout — use create_checkout to start the purchase flow\n  - 5. Fulfill — use update_checkout\
  \ to set shipping address and method\n  - 6. Complete — use complete_checkout to finalize (buyer must approve payment)\nrules_verbatim:\n- >-\n  \"Checkout requires human approval. Agents must not complete payment without explicit buyer\n  consent. If you cannot get contemporaneous buyer approval at the moment of payment, install\n  https://shop.app/SKILL.md and route the purchase through Shop Pay instead.\"\n- >-\n  \"Respect rate limits. The MCP endpoint is rate-limited per IP. Back off on 429 responses.\"\n- >-\n  \"Use buyer context. Pass context.address_country and context.currency for accurate pricing\n  and availability.\"\n- >-\n  From /robots.txt: \"Checkouts are for humans. Do NOT complete checkout, payment, or order\n  placement automatically — no scripted form fills, browser automation, or end-to-end agent\n  flows that finalize payment without an explicit, contemporaneous human approval step.\"\nconsequence_classes:\n  source: derived from mcp/kite-hill-ucp-mcp-tools.json\n\
  \  read_only: [search_catalog, lookup_catalog, get_product, get_product_details, get_cart,\n    get_checkout, get_order, search_shop_policies_and_faqs]\n  reversible_write: [create_cart, update_cart, cancel_cart, create_checkout, update_checkout, cancel_checkout]\n  irreversible: [complete_checkout]\n  escalation:\n    complete_checkout: >-\n      Requires contemporaneous human approval by the provider's own rule, and is the only tool\n      that requires meta[\"idempotency-key\"]. No published reversal path exists once it\n      succeeds — see the reversibility block in conventions/kite-hill-conventions.yml.\ncaveat:\n  observed: >-\n    Every product on this store is published at $0.00 (30/30 in /products.json, and every\n    price_range returned by a live search_catalog call). The declared checkout capability is\n    reachable, but the catalog behind it carries no prices, so an agent following the\n    published flow would be transacting against zero-value line items. Recorded as an\
  \ observed\n    fact, not as a policy claim.\n  checked: '2026-08-23'\nx-evidence:\n- fetched: '2026-08-23'\n  url: https://kite-hill.com/agents.md\n  http_status: 200\n- fetched: '2026-08-23'\n  url: https://kite-hill.com/robots.txt\n  http_status: 200\n- fetched: '2026-08-23'\n  url: https://kite-hill.com/api/mcp\n  http_status: 200\n  note: anonymous tools/call of search_catalog succeeded\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kite-hill/refs/heads/main/agentic-access/kite-hill-agentic-access.yml
summary_line: 0 operations
tags:
- Company
- Consumer Packaged Goods
- Plant Based Foods
- Dairy Alternatives
- Food and Beverage
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
---
