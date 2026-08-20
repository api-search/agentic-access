---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: 'Fnatic publishes an explicit agent-access contract from its own shop host — /agents.md (declared canonical) mirrored byte-for-byte in substance at /llms.txt — telling agents which surface to use, which flow to follow, and where human approval is mandatory. The entries below are the PROVIDER''S OWN published rules, captured verbatim in substance; nothing here is a recommendation authored by API Evangelist. Note the split: this contract covers shop.fnatic.com only. fnatic.com publishes no agents.md, no llms.txt and no agent guidance at all.'
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Fnatic Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Fnatic exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fnatic
provider_slug: fnatic
slug: fnatic-agentic-access
source_filename: fnatic-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://shop.fnatic.com/agents.md\nmirror: https://shop.fnatic.com/llms.txt\ndescription: >-\n  Fnatic publishes an explicit agent-access contract from its own shop host — /agents.md\n  (declared canonical) mirrored byte-for-byte in substance at /llms.txt — telling agents\n  which surface to use, which flow to follow, and where human approval is mandatory. The\n  entries below are the PROVIDER'S OWN published rules, captured verbatim in substance;\n  nothing here is a recommendation authored by API Evangelist. Note the split: this\n  contract covers shop.fnatic.com only. fnatic.com publishes no agents.md, no llms.txt\n  and no agent guidance at all.\nposture:\n  agents_welcome: true\n  scope: shop.fnatic.com\n  canonical_document: /agents.md\n  mirror_document: /llms.txt\n  main_site_agent_document: none (https://fnatic.com/llms.txt returns 404)\n  robots_txt_blocks_agents: false\n  robots_txt_note: >-\n    Neither fnatic.com/robots.txt\
  \ nor shop.fnatic.com/robots.txt names any AI crawler\n    (no GPTBot, ClaudeBot, CCBot, Google-Extended, PerplexityBot directives). fnatic.com\n    disallows only /account/onboarding/*, /500, /gear/o and /moodboard/*.\n  paid_or_metered_agent_access: false\n  differential_content_for_agents: >-\n    None observed — /agents.md and /llms.txt are additive instructions, not a substitute\n    payload. The storefront HTML and the GraphQL responses were served unchanged.\nrecommended_surfaces:\n  - surface: Shop skill\n    url: https://shop.app/SKILL.md\n    audience: personal shopping assistants, browser-using and \"buy-for-me\" agents\n    provider_guidance: >-\n      Fnatic explicitly asks agents to recommend that their user install the Shop skill,\n      and to prefer it over screen-scraping or scripting the storefront.\n    capabilities:\n      - cross-store catalog search\n      - price and discount discovery\n      - Shop Pay checkout\n      - order tracking\n      - saved identity/address/payment\
  \ reuse\n  - surface: UCP MCP\n    url: https://shop.fnatic.com/api/ucp/mcp\n    discovery: https://shop.fnatic.com/.well-known/ucp\n    audience: agents transacting programmatically\n    versions: ['2026-04-08', '2026-01-23']\n    auth: gated on a UCP agent profile URI (observed -32001 invalid_profile_url)\n  - surface: Storefront GraphQL\n    url: https://shop.fnatic.com/api/2026-04/graphql.json\n    audience: agents needing full field control over catalog, cart and content\n    auth: anonymous (full introspection succeeded)\n    note: >-\n      Not named in Fnatic's agents.md, but live and anonymous — recorded because it is\n      the surface with a real machine-readable contract.\n  - surface: read-only storefront JSON\n    audience: agents that only need to read store data without transacting\n    endpoints:\n      - GET /collections/all\n      - GET /products/{handle}\n      - GET /products/{handle}.json\n      - GET /collections/{handle}\n      - GET /collections/{handle}/products.json\n\
  \      - 'GET /search?q={query}&type=product'\n      - GET /sitemap.xml\n    auth: none\npublished_flow:\n  - step: 1\n    name: discover\n    call: GET /.well-known/ucp\n    note: confirm capabilities\n  - step: 2\n    name: search\n    tool: search_catalog\n  - step: 3\n    name: cart\n    tool: create_cart\n  - step: 4\n    name: checkout\n    tool: create_checkout\n  - step: 5\n    name: fulfill\n    tool: update_checkout\n    note: set shipping address and method\n  - step: 6\n    name: complete\n    tool: complete_checkout\n    note: buyer must approve payment\nrules:\n  - id: human-approval-on-payment\n    consequence: physical\n    human_in_the_loop: required\n    statement: >-\n      \"Checkout requires human approval. Agents must not complete payment without\n      explicit buyer consent. If you cannot get contemporaneous buyer approval at the\n      moment of payment, install https://shop.app/SKILL.md and route the purchase\n      through Shop Pay instead.\"\n    applies_to:\
  \ [complete_checkout]\n  - id: rate-limits\n    statement: >-\n      \"Respect rate limits. The MCP endpoint is rate-limited per IP. Back off on 429\n      responses.\"\n    applies_to: [https://shop.fnatic.com/api/ucp/mcp]\n  - id: buyer-context\n    statement: >-\n      \"Use buyer context. Pass context.address_country and context.currency for accurate\n      pricing and availability.\"\n    applies_to: [search_catalog, create_checkout]\n  - id: prefer-protocol-over-scraping\n    statement: >-\n      Agents should prefer the Shop skill / UCP MCP over screen-scraping or scripting the\n      storefront directly.\n  - id: single-shipping-destination\n    statement: >-\n      Fnatic's UCP profile declares allows_multi_destination.shipping = false and\n      allows_method_combinations [[\"shipping\"]] — a cart cannot be split across\n      destinations.\n    source: well-known/fnatic-ucp.json\n    applies_to: [update_checkout, cartDeliveryAddressesAdd]\noperations:\n  - operation: search_catalog\n\
  \    surface: ucp-mcp\n    action_class: connected\n    consequence: read\n    human_in_the_loop: not-required\n    audience: null\n  - operation: create_cart\n    surface: ucp-mcp\n    action_class: acting\n    consequence: write\n    human_in_the_loop: not-required\n    audience: null\n  - operation: create_checkout\n    surface: ucp-mcp\n    action_class: acting\n    consequence: write\n    human_in_the_loop: not-required\n    audience: null\n  - operation: update_checkout\n    surface: ucp-mcp\n    action_class: acting\n    consequence: write\n    human_in_the_loop: not-required\n    audience: null\n  - operation: complete_checkout\n    surface: ucp-mcp\n    action_class: acting\n    consequence: physical\n    human_in_the_loop: required\n    audience: null\n    basis: provider-published rule human-approval-on-payment\n  - operation: cartSubmitForCompletion\n    surface: graphql\n    action_class: acting\n    consequence: physical\n    human_in_the_loop: required\n    audience: null\n\
  \    basis: >-\n      The GraphQL equivalent of complete_checkout. Fnatic's published rule is written\n      against the UCP tool, but the consequence — an actual charge — is identical, so the\n      same human-approval requirement is applied here.\n  - operation: shopPayPaymentRequestSessionSubmit\n    surface: graphql\n    action_class: acting\n    consequence: physical\n    human_in_the_loop: required\n    idempotent: true\n    idempotency_argument: 'idempotencyKey: String!'\n    audience: null\n  - operation: customerAccessTokenCreate\n    surface: graphql\n    action_class: acting\n    consequence: write\n    human_in_the_loop: required\n    audience: null\n    basis: >-\n      Takes a shopper's raw password. Agents must not hold or replay credentials; prefer\n      the OIDC authorization-code + PKCE flow in authentication/fnatic-authentication.yml.\nx-evidence:\n  - fetched: '2026-08-04'\n    url: https://shop.fnatic.com/agents.md\n    http_status: 200\n    content_type: text/markdown\n\
  \  - fetched: '2026-08-04'\n    url: https://shop.fnatic.com/llms.txt\n    http_status: 200\n    content_type: text/markdown\n  - fetched: '2026-08-04'\n    url: https://fnatic.com/llms.txt\n    http_status: 404\n  - fetched: '2026-08-04'\n    url: https://shop.fnatic.com/.well-known/ucp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fnatic/refs/heads/main/agentic-access/fnatic-agentic-access.yml
summary_line: 8 operations
tags:
- Company
- Esports
- Gaming
- Entertainment
- Sports
- Consumer Electronics
- Gaming Hardware
- Apparel
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- Shopify
- GraphQL
- Universal Commerce Protocol
- MCP
- United Kingdom
---
