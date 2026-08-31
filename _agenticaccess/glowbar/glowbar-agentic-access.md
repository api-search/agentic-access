---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Glowbar Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Glowbar exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Glowbar
provider_slug: glowbar
slug: glowbar-agentic-access
source_filename: glowbar-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: generated\nsource: mcp/glowbar-mcp-tools.json + https://glowbar.com/robots.txt + https://glowbar.com/agents.md + https://glowbar.com/llms.txt\nnote: >-\n  A recommended x-agentic-access contract, classified per MCP tool. The tool names, required\n  parameters and consequence-bearing behaviours are read from the live tools/list response; the\n  escalation rules restate the provider's OWN published agent policy, which it states in three\n  places (robots.txt, agents.md, llms.txt). Nothing here is a policy API Evangelist invented on\n  Glowbar's behalf — where the provider is silent, the field says so.\nprovider_stated_policy:\n  agent_access_permitted: true\n  sanctioned_interfaces:\n  - https://glowbar.com/api/ucp/mcp\n  - https://shop.app/SKILL.md\n  prohibited:\n  - Scripted form fills against the HTML checkout\n  - Browser automation that finalizes payment\n  - End-to-end agent flows that complete payment without contemporaneous human approval\n\
  \  human_approval_required_for: [payment, checkout completion, order placement]\n  quote: 'Checkouts are for humans. Do NOT complete checkout, payment, or order placement automatically.'\n  sources:\n  - url: https://glowbar.com/robots.txt\n    http_status: 200\n  - url: https://glowbar.com/agents.md\n    http_status: 200\n  - url: https://glowbar.com/llms.txt\n    http_status: 200\n  crawl_policy:\n    robots_allow: true\n    note: 'robots.txt Allow: / for User-agent: *. Public product, collection, page, blog, policy, cart and localized HTML is explicitly declared crawlable.'\nidentity:\n  required: true\n  mechanism: meta.ucp-agent.profile — a dereferenceable agent profile URI\n  anonymous_discovery_permitted: true\n  note: Agents must identify themselves with a fetchable profile on every call, but need no credential to discover the tool set.\noperations:\n- tool: search_catalog\n  action_class: read\n  consequence: none\n  reversible: na\n  token: none\n  escalation: none\n- tool: lookup_catalog\n\
  \  action_class: read\n  consequence: none\n  reversible: na\n  token: none\n  escalation: none\n- tool: get_product\n  action_class: read\n  consequence: none\n  reversible: na\n  token: none\n  escalation: none\n- tool: get_cart\n  action_class: read\n  consequence: none\n  reversible: na\n  token: none\n  escalation: none\n- tool: get_checkout\n  action_class: read\n  consequence: none\n  reversible: na\n  token: none\n  escalation: none\n- tool: get_order\n  action_class: read\n  consequence: none\n  reversible: na\n  token: none\n  escalation: none\n  note: Buyer-scoped; anonymous callers can only read orders they created in-session.\n- tool: create_cart\n  action_class: write\n  consequence: low\n  reversible: true\n  reversal: cancel_cart\n  token: none\n  escalation: none\n  rationale: Creates no financial obligation and is undone by a published tool.\n- tool: update_cart\n  action_class: write\n  consequence: low\n  reversible: true\n  reversal: update_cart\n  token: none\n  escalation:\
  \ none\n- tool: cancel_cart\n  action_class: write\n  consequence: low\n  reversible: false\n  token: none\n  escalation: none\n  rationale: Destructive but only of a draft basket; no buyer harm.\n- tool: create_checkout\n  action_class: write\n  consequence: medium\n  reversible: true\n  reversal: cancel_checkout\n  token: none\n  escalation: notify\n  rationale: Reserves nothing and charges nothing, but begins a purchase flow the buyer should be aware of.\n- tool: update_checkout\n  action_class: write\n  consequence: medium\n  reversible: true\n  reversal: update_checkout\n  token: none\n  escalation: notify\n  note: Carries the shipping address, so it moves buyer PII.\n- tool: cancel_checkout\n  action_class: write\n  consequence: low\n  reversible: false\n  token: none\n  escalation: none\n- tool: complete_checkout\n  action_class: write\n  consequence: high-financial\n  reversible: false\n  reversal: none-via-api\n  out_of_band_remedy: 'Exchange or store credit on unopened retail\
  \ product within 21 days (https://glowbar.com/policies/refund-policy)'\n  token: meta.idempotency-key (required by schema)\n  escalation: human-approval-required\n  approval_type: explicit, contemporaneous buyer approval at the moment of payment\n  rationale: >-\n    The only operation that moves money and the only one with no API reversal. The provider\n    mandates human approval, the schema mandates an idempotency key, and the remedy afterwards\n    is a manual returns process yielding store credit rather than a refund. An agent must treat\n    this as a one-way door.\n  provider_stated: true\nsummary:\n  tool_count: 13\n  read: 6\n  write_low: 4\n  write_medium: 2\n  write_high_financial: 1\n  requiring_human_approval: 1\n  requiring_idempotency_token: 1\n  irreversible: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glowbar/refs/heads/main/agentic-access/glowbar-agentic-access.yml
summary_line: 13 operations
tags:
- Company
- Skincare
- Beauty
- Retail
- Commerce
- E-Commerce
- Consumer Services
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Memberships
---
