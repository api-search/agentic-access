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
name: Voyage Foods Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Voyage Foods exposes 13 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read, 5 write, and 3 physical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Voyage Foods
provider_slug: voyage-foods
slug: voyage-foods-agentic-access
source_filename: voyage-foods-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: >-\n  https://voyagefoods.com/agents.md, https://voyagefoods.com/llms.txt and\n  https://voyagefoods.com/robots.txt — the store publishes its own agent access policy in prose, and\n  the operation classifications below are bound to the 13 real tools returned by\n  https://voyagefoods.com/api/ucp/mcp tools/list.\nnote: >-\n  Unlike most entries in this catalog, the access contract here is NOT generated from an OpenAPI by\n  derive-agentic-access.py — this provider publishes no OpenAPI. It is read from an agent policy the\n  merchant actually publishes, in three places, and cross-checked against the live tool schemas.\n  Fields marked provider_stated are quoted from that policy; fields marked derived are this\n  pipeline's classification of the tool.\npublished_policy:\n  agent_policy_documents:\n  - {url: 'https://voyagefoods.com/agents.md', status: 200, content_type: text/markdown}\n  - {url: 'https://voyagefoods.com/llms.txt',\
  \ status: 200, content_type: text/markdown}\n  - {url: 'https://voyagefoods.com/robots.txt', status: 200, content_type: text/plain}\n  crawl_posture: >-\n    robots.txt allows all user-agents across product, collection, page, blog, policy, cart and\n    localized HTML. No AI-crawler blocks were observed.\n  agent_identity_required: true\n  agent_identity_mechanism: meta[\"ucp-agent\"].profile — a dereferenceable agent profile URI\n  human_approval_required_for_payment: true\n  provider_statements:\n  - >-\n      \"Checkout requires human approval. Agents must not complete payment without explicit buyer\n      consent. If you cannot get contemporaneous buyer approval at the moment of payment, install\n      https://shop.app/SKILL.md and route the purchase through Shop Pay instead.\"\n  - >-\n      \"Checkouts are for humans. Do NOT complete checkout, payment, or order placement automatically\n      — no scripted form fills, browser automation, or end-to-end agent flows that finalize payment\n\
  \      without an explicit, contemporaneous human approval step.\"\n  - >-\n      \"Respect rate limits. The MCP endpoint is rate-limited per IP. Back off on 429 responses.\"\n  - >-\n      \"Use buyer context. Pass context.address_country and context.currency for accurate pricing and\n      availability.\"\n  preferred_channel: >-\n    The store explicitly prefers the UCP/MCP endpoints or the Shop skill over screen-scraping or\n    scripting the storefront: \"If your user permits installation, you should prefer the Shop skill\n    over screen-scraping or scripting the storefront directly.\"\nsummary:\n  operations_classified: 13\n  by_action_class: {connected: 5, acting: 8}\n  by_consequence: {read: 5, write: 5, physical: 3}\n  human_in_the_loop_required: 1\n  audit_required: 8\n  agent_identity_required: 13\noperations:\n- operation: search_catalog\n  action_class: connected\n  consequence: read\n  audience: null\n  human_in_the_loop: not-required\n  audit: optional\n  basis: derived\n\
  - operation: lookup_catalog\n  action_class: connected\n  consequence: read\n  audience: null\n  human_in_the_loop: not-required\n  audit: optional\n  basis: derived\n- operation: get_product\n  action_class: connected\n  consequence: read\n  audience: null\n  human_in_the_loop: not-required\n  audit: optional\n  basis: derived\n- operation: get_cart\n  action_class: connected\n  consequence: read\n  audience: null\n  human_in_the_loop: not-required\n  audit: optional\n  basis: derived\n- operation: get_checkout\n  action_class: connected\n  consequence: read\n  audience: null\n  human_in_the_loop: not-required\n  audit: optional\n  basis: derived\n- operation: get_order\n  action_class: connected\n  consequence: read\n  audience: null\n  human_in_the_loop: not-required\n  audit: required\n  basis: derived\n  note: Returns buyer order detail; read-only but personally identifying.\n- operation: create_cart\n  action_class: acting\n  consequence: write\n  audience: null\n  human_in_the_loop:\
  \ not-required\n  audit: required\n  basis: derived\n- operation: update_cart\n  action_class: acting\n  consequence: write\n  audience: null\n  human_in_the_loop: not-required\n  audit: required\n  basis: derived\n- operation: cancel_cart\n  action_class: acting\n  consequence: write\n  audience: null\n  human_in_the_loop: not-required\n  audit: required\n  basis: derived\n- operation: create_checkout\n  action_class: acting\n  consequence: write\n  audience: null\n  human_in_the_loop: not-required\n  audit: required\n  basis: derived\n- operation: update_checkout\n  action_class: acting\n  consequence: write\n  audience: null\n  human_in_the_loop: not-required\n  audit: required\n  basis: derived\n  note: >-\n    Accepts payment.instruments including credential tokens and billing addresses — treat as\n    handling payment material even though it does not authorize a charge.\n- operation: cancel_checkout\n  action_class: acting\n  consequence: physical\n  audience: null\n  human_in_the_loop:\
  \ not-required\n  audit: required\n  basis: derived\n  note: Voids a checkout that may already hold buyer payment instruments.\n- operation: complete_checkout\n  action_class: acting\n  consequence: physical\n  audience: null\n  human_in_the_loop: required\n  human_in_the_loop_basis: provider_stated\n  idempotency_key: required\n  idempotency_field: meta[\"idempotency-key\"]\n  audit: required\n  basis: derived\n  note: >-\n    The only operation the merchant's own published policy gates on contemporaneous human approval.\n    It moves money and creates an order. The store names an alternative route (the Shop skill via\n    Shop Pay) for agents that cannot obtain approval in the moment.\nescalation:\n  continue_url: >-\n    Every UCP error envelope carries data.continue_url (observed:\n    https://voyage-foods-2021.myshopify.com/), a human-resumable URL the agent can hand to the buyer\n    when it cannot proceed. This is a real, observed handoff path rather than a documented one.\ngaps:\n\
  \  - No published token TTL, scope-per-operation, or proof-of-possession requirement for the agent JWT.\n  - No published audit or retention commitment; audit values above are this pipeline's recommendation.\n  - No agent-profile schema is published, so the shape of a conforming meta[\"ucp-agent\"].profile document is unstated.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - {url: 'https://voyagefoods.com/agents.md', http_status: 200}\n  - {url: 'https://voyagefoods.com/llms.txt', http_status: 200}\n  - {url: 'https://voyagefoods.com/robots.txt', http_status: 200}\n  - {url: 'https://voyagefoods.com/api/ucp/mcp', http_status: 200, note: 'tools/list returned 13 tools'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyage-foods/refs/heads/main/agentic-access/voyage-foods-agentic-access.yml
summary_line: 13 operations · 8 acting · 1 human-in-the-loop
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Ecommerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
- Shopify
- Food Technology
---
