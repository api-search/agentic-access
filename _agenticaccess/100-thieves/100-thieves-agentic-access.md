---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
consequence_counts:
  financial: 1
  read: 6
  write: 6
description: ''
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: searched
name: 100 Thieves Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: '100 Thieves exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 6 write.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 100 Thieves
provider_slug: 100-thieves
slug: 100-thieves-agentic-access
source_filename: 100-thieves-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource:\n- https://100thieves.com/agents.md\n- https://100thieves.com/robots.txt\n- https://100thieves.com/llms.txt\n- mcp/100-thieves-tools-list.json\nnote: >-\n  Unlike most entries in the catalog, this is not a generated governance starting\n  point — 100 Thieves (via its Shopify UCP storefront) actually publishes agent access\n  rules, so the contract below is transcribed from the provider's own statements and\n  from the live tool schemas. derive-agentic-access.py was not run: it reads openapi/,\n  and there is no OpenAPI here.\nprovider_published_policy:\n  canonical_document: https://100thieves.com/agents.md\n  mirrors: [https://100thieves.com/llms.txt]\n  advertised_in: [robots.txt]\n  rules:\n  - id: buyer-approval-invariant\n    statement: >-\n      \"Checkouts are for humans. Do NOT complete checkout, payment, or order placement\n      automatically — no scripted form fills, browser automation, or end-to-end agent\n    \
  \  flows that finalize payment without an explicit, contemporaneous human approval\n      step.\"\n    source: https://100thieves.com/robots.txt\n  - id: sanctioned-transaction-paths\n    statement: Agents transacting on a buyer's behalf must use the UCP/MCP endpoint\n      or the Shop skill; both require buyer approval before payment.\n    paths: [https://100thieves.com/api/ucp/mcp, https://shop.app/SKILL.md]\n  - id: rate-limits\n    statement: The MCP endpoint is rate-limited per IP. Back off on 429 responses.\n  - id: buyer-context\n    statement: Pass context.address_country and context.currency for accurate pricing\n      and availability.\n  - id: crawling-permitted\n    statement: Public product, collection, page, blog, policy, cart, and localized\n      HTML is crawlable.\n  - id: prefer-protocol-over-scraping\n    statement: Agents should prefer the UCP/MCP endpoints or the Shop skill over screen-scraping\n      or scripting the storefront directly.\n  contact: bots@shopify.com\n\
  agent_identity:\n  required: true\n  mechanism: UCP agent profile\n  field: meta.ucp-agent.profile\n  format: URI\n  enforcement: >-\n    Enforced server-side. A tools/call without a resolvable profile URI returns JSON-RPC\n    -32001 \"UCP discovery failed\" / invalid_profile_url with HTTP 422 — observed live.\n    tools/list itself is anonymous.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 6\n    acting: 7\n  by_consequence:\n    read: 6\n    write: 6\n    financial: 1\n  human_in_the_loop_required: 1\noperations:\n- tool: search_catalog\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n- tool: lookup_catalog\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n- tool: get_product\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n- tool: get_cart\n  action_class: connected\n  consequence: read\n  audit: optional\n\
  \  human_in_the_loop: not-required\n- tool: get_checkout\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n- tool: get_order\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n  note: Reads buyer order data — treat the order id as a bearer capability.\n- tool: create_cart\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: not-required\n- tool: update_cart\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: not-required\n- tool: cancel_cart\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: not-required\n- tool: create_checkout\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: not-required\n- tool: update_checkout\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: not-required\n  note: Carries shipping address\
  \ — PII enters the call here.\n- tool: cancel_checkout\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: not-required\n- tool: complete_checkout\n  action_class: acting\n  consequence: financial\n  audit: required\n  human_in_the_loop: required\n  escalation: buyer-approval\n  note: >-\n    The one operation the provider explicitly fences. Payment is finalized here and\n    the store's published policy forbids completing it without explicit, contemporaneous\n    human approval. Agents that cannot obtain that approval are directed to route the\n    purchase through Shop Pay via the Shop skill.\naudience: null\nx-evidence:\n- url: https://100thieves.com/agents.md\n  http_status: 200\n- url: https://100thieves.com/robots.txt\n  http_status: 200\n- url: https://100thieves.com/api/ucp/mcp\n  http_status: 422\n  note: agent-profile gate observed on tools/call\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/100-thieves/refs/heads/main/agentic-access/100-thieves-agentic-access.yml
summary_line: 13 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- Esports
- Gaming
- Apparel
- Retail
- E-Commerce
- Entertainment
- Media
- Direct to Consumer
- Agentic Commerce
---
