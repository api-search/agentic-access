---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 5
consequence_counts:
  financial: 1
  read: 5
  write: 7
description: ''
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: searched
name: Quip Nyc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Quip NYC exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 7 write.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quip NYC
provider_slug: quip-nyc
slug: quip-nyc-agentic-access
source_filename: quip-nyc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource:\n- https://www.getquip.com/agents.md\n- https://www.getquip.com/llms.txt\n- https://www.getquip.com/robots.txt\n- mcp/quip-nyc-tools-list.json\nnote: >-\n  This is not a generated governance starting point — quip, via its Shopify UCP storefront,\n  actually publishes agent access rules, so the contract below is transcribed from the\n  provider's own statements and from the live tool schemas. derive-agentic-access.py was not\n  run: it reads openapi/, and there is no OpenAPI here.\nprovider_published_policy:\n  canonical_document: https://www.getquip.com/agents.md\n  mirrors: [https://www.getquip.com/llms.txt]\n  rules:\n  - id: buyer-approval-invariant\n    statement: >-\n      \"Checkout requires human approval. Agents must not complete payment without explicit\n      buyer consent. If you cannot get contemporaneous buyer approval at the moment of\n      payment, install https://shop.app/SKILL.md and route the purchase through\
  \ Shop Pay\n      instead.\"\n    source: https://www.getquip.com/agents.md\n  - id: sanctioned-transaction-paths\n    statement: >-\n      Agents transacting on a buyer's behalf should use the UCP/MCP endpoint or the Shop\n      skill; both require buyer approval before payment.\n    paths: [https://www.getquip.com/api/ucp/mcp, https://shop.app/SKILL.md]\n  - id: rate-limits\n    statement: The MCP endpoint is rate-limited per IP. Back off on 429 responses.\n  - id: buyer-context\n    statement: >-\n      Pass context.address_country and context.currency for accurate pricing and availability.\n  - id: prefer-protocol-over-scraping\n    statement: >-\n      \"If your user permits installation, you should prefer the Shop skill over\n      screen-scraping or scripting the storefront directly.\"\n  - id: read-only-surface-is-open\n    statement: >-\n      Agents that only need to read store data may use /collections/all,\n      /products/{handle}.json, /collections/{handle}/products.json\
  \ and /sitemap.xml with no\n      authentication.\n  - id: money-format\n    statement: >-\n      Prices are integer ISO 4217 minor units paired with a currency code; convert before\n      quoting a price to a buyer.\n    note: Stated on all thirteen tools, not only the transacting ones.\nagent_identity:\n  required: true\n  mechanism: UCP agent profile\n  field: meta.ucp-agent.profile\n  format: URI\n  enforcement: >-\n    Enforced server-side. A tools/call without a resolvable profile URI returns JSON-RPC\n    -32001 \"UCP discovery failed\" / invalid_profile_url with HTTP 422 — observed live on\n    2026-08-26. tools/list and initialize are anonymous.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 5\n    acting: 8\n  by_consequence:\n    read: 5\n    write: 7\n    financial: 1\n  human_in_the_loop_required: 1\n  reversible: 2\n  irreversible_writes: 1\noperations:\n- tool: search_catalog\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop:\
  \ not-required\n  reversible: na\n- tool: lookup_catalog\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n  reversible: na\n- tool: get_product\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n  reversible: na\n- tool: get_cart\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n  reversible: na\n- tool: get_checkout\n  action_class: connected\n  consequence: read\n  audit: optional\n  human_in_the_loop: not-required\n  reversible: na\n- tool: get_order\n  action_class: connected\n  consequence: read\n  audit: recommended\n  human_in_the_loop: not-required\n  reversible: na\n  note: Returns a real customer order record; treat the response as personal data.\n- tool: create_cart\n  action_class: acting\n  consequence: write\n  audit: recommended\n  human_in_the_loop: not-required\n  reversible: yes\n  reversal: cancel_cart\n- tool:\
  \ update_cart\n  action_class: acting\n  consequence: write\n  audit: recommended\n  human_in_the_loop: not-required\n  reversible: yes\n  reversal: cancel_cart\n- tool: cancel_cart\n  action_class: acting\n  consequence: write\n  audit: recommended\n  human_in_the_loop: not-required\n  reversible: no\n  note: This IS the reversal. Cancelling is itself not undoable — create a new cart.\n- tool: create_checkout\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: recommended\n  reversible: yes\n  reversal: cancel_checkout\n- tool: update_checkout\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: recommended\n  reversible: yes\n  reversal: cancel_checkout\n  note: Sets shipping address and delivery method — personal data enters here.\n- tool: cancel_checkout\n  action_class: acting\n  consequence: write\n  audit: required\n  human_in_the_loop: not-required\n  reversible: no\n  note: This IS the reversal.\n- tool: complete_checkout\n\
  \  action_class: acting\n  consequence: financial\n  audit: required\n  human_in_the_loop: required\n  escalation: >-\n    quip's published rule: an agent must obtain explicit, contemporaneous buyer approval at\n    the moment of payment, or route the purchase through Shop Pay via the Shop skill.\n  reversible: no\n  reversal: null\n  note: >-\n    The single irreversible action on the surface. No refund, void or order-cancel tool\n    exists in the tool set and no order mutation exists in the Storefront GraphQL schema.\n    Reversal is a human channel only — email help@getquip.com within 30 days per\n    https://www.getquip.com/policies/refund-policy.\nx-evidence:\n- url: https://www.getquip.com/agents.md\n  status: 200\n- url: https://www.getquip.com/api/ucp/mcp\n  status: 200\n  note: tools/list — all 13 tools and schemas\n- url: https://www.getquip.com/api/ucp/mcp\n  status: 422\n  note: tools/call without agent profile — identity gate observed\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quip-nyc/refs/heads/main/agentic-access/quip-nyc-agentic-access.yml
summary_line: 13 operations · 8 acting · 1 human-in-the-loop
tags:
- Company
- Oral Care
- Consumer Health
- Personal Care
- Retail
- E-Commerce
- Direct to Consumer
- Subscription
- Agentic Commerce
- Shopify
---
