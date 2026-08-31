---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Prime Hydration Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Prime Hydration exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Prime Hydration
provider_slug: prime-hydration
slug: prime-hydration-agentic-access
source_filename: prime-hydration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://drinkprime.com/robots.txt (HTTP 200),\n  https://drinkprime.com/llms.txt (HTTP 200),\n  https://drinkprime.com/agents.md (HTTP 200),\n  https://drinkprime.com/sitemap_agentic_discovery.xml (HTTP 200),\n  and the live tool set at https://drinkprime.com/api/ucp/mcp - all probed 2026-08-26.\nnote: >-\n  This is a SEARCHED artifact, not a generated recommendation. Prime Hydration publishes an\n  explicit, unusually specific agent-access policy in three places that agree with each other,\n  and it draws the line exactly where it matters: reading and cart-building are invited,\n  finalising payment without a human is forbidden. The policy text below is quoted verbatim\n  from the provider's own files.\nposture: invited-with-a-hard-stop\ndiscovery:\n  robots_txt: https://drinkprime.com/robots.txt\n  agents_md: https://drinkprime.com/agents.md\n  llms_txt: https://drinkprime.com/llms.txt\n  agentic_sitemap: https://drinkprime.com/sitemap_agentic_discovery.xml\n\
  \  ucp_profile: https://drinkprime.com/.well-known/ucp\n  mcp_endpoint: https://drinkprime.com/api/ucp/mcp\n  canonical: >-\n    agents.md is named canonical; llms.txt mirrors it. /sitemap_agentic_discovery.xml exists for\n    the sole purpose of pointing crawlers at /agents.md.\ncrawl_policy:\n  robots_user_agent: '*'\n  default: Allow /\n  ai_crawlers_blocked: false\n  note: >-\n    No GPTBot, ClaudeBot, CCBot, PerplexityBot or Google-Extended block. Public product,\n    collection, page, blog, policy, cart and localized HTML is explicitly declared crawlable.\n  disallowed:\n  - /admin\n  - /cart/\n  - /checkout\n  - /checkouts/\n  - /orders\n  - /account\n  - /services\n  - /sf_*\n  - /cart.js\n  - /recommendations/products\n  ajax_note: >-\n    The AJAX surfaces /cart.js and /recommendations/products are deliberately disallowed with\n    the comment \"agents should use UCP/MCP instead\" - a redirection of agents onto the\n    supported contract rather than a block.\npolicy_quotes:\n\
  - source: https://drinkprime.com/robots.txt\n  text: >-\n    Checkouts are for humans. Do NOT complete checkout, payment, or order placement\n    automatically - no scripted form fills, browser automation, or end-to-end agent flows that\n    finalize payment without an explicit, contemporaneous human approval step. Agents\n    transacting on a buyer's behalf must use the UCP/MCP endpoints above or the Shopify shopping\n    skill (https://shop.app/SKILL.md); both require buyer approval before payment.\n- source: https://drinkprime.com/llms.txt\n  text: >-\n    Checkout requires human approval. Agents must not complete payment without explicit buyer\n    consent. If you cannot get contemporaneous buyer approval at the moment of payment, install\n    https://shop.app/SKILL.md and route the purchase through Shop Pay instead.\n- source: https://drinkprime.com/llms.txt\n  text: >-\n    Respect rate limits. The MCP endpoint is rate-limited per IP. Back off on 429 responses.\noperations:\n- tool:\
  \ search_catalog\n  action_class: read\n  consequence: none\n  escalation: none\n  token: anonymous\n- tool: lookup_catalog\n  action_class: read\n  consequence: none\n  escalation: none\n  token: anonymous\n- tool: get_product\n  action_class: read\n  consequence: none\n  escalation: none\n  token: anonymous\n- tool: get_cart\n  action_class: read\n  consequence: none\n  escalation: none\n  token: anonymous\n- tool: get_checkout\n  action_class: read\n  consequence: none\n  escalation: none\n  token: anonymous\n- tool: get_order\n  action_class: read\n  consequence: none\n  escalation: none\n  token: anonymous\n- tool: create_cart\n  action_class: write\n  consequence: reversible\n  reversal: cancel_cart\n  escalation: none\n  token: anonymous\n- tool: update_cart\n  action_class: write\n  consequence: reversible\n  reversal: cancel_cart\n  escalation: none\n  token: anonymous\n- tool: cancel_cart\n  action_class: write\n  consequence: reversible\n  escalation: none\n  token: anonymous\n\
  - tool: create_checkout\n  action_class: write\n  consequence: reversible\n  reversal: cancel_checkout\n  escalation: none\n  token: anonymous\n- tool: update_checkout\n  action_class: write\n  consequence: reversible\n  reversal: cancel_checkout\n  escalation: none\n  token: anonymous\n- tool: cancel_checkout\n  action_class: write\n  consequence: reversible\n  escalation: none\n  token: anonymous\n- tool: complete_checkout\n  action_class: transact\n  consequence: irreversible\n  reversal: none\n  refund_available: false\n  refund_policy: https://drinkprime.com/policies/refund-policy\n  escalation: human-approval-required\n  escalation_basis: provider-published (robots.txt and llms.txt, verbatim above)\n  idempotency_key: required (meta.idempotency-key)\n  token: anonymous + buyer-authorized payment handler\nrecommended_agent_contract:\n  - Read /agents.md before acting; it is the canonical instruction document.\n  - Send meta.ucp-agent.profile on every call.\n  - Treat 429 as a hard\
  \ backoff signal; no numeric budget is published.\n  - Never call complete_checkout without contemporaneous, explicit buyer approval.\n  - Always supply meta.idempotency-key on complete_checkout; a retry without it may double-charge.\n  - Know before you act that the purchase is final sale - there is no refund tool and no refund policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prime-hydration/refs/heads/main/agentic-access/prime-hydration-agentic-access.yml
summary_line: 13 operations
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Food and Beverage
- Retail
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Sports Nutrition
---
