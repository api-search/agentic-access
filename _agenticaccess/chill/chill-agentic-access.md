---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: searched
name: Chill Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 0
overview: 'Chill exposes 0 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chill
provider_slug: chill
slug: chill-agentic-access
source_filename: chill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://chill.com/llms.txt + https://chill.com/.well-known/ucp\naudience: null\nsummary: >-\n  Chill.com publishes real agent-access guidance: an llms.txt agent guide plus a\n  Universal Commerce Protocol (UCP) merchant profile and MCP endpoint. This captures\n  the provider's own stated execution contract for AI agents, not a derived one.\naccess_classes:\n- class: connected\n  consequence: read\n  operations: [browse products, product JSON, collection JSON, catalog search/lookup]\n  auth_required: false\n  note: Read-only browsing needs no authentication.\n- class: acting\n  consequence: physical\n  operations: [create_cart, create_checkout, update_checkout, complete_checkout]\n  auth_required: true\n  auth: Shopify Customer Account OAuth (customer-account-mcp-api:full)\n  human_in_the_loop: required\n  note: >-\n    Checkout / payment completion requires explicit, contemporaneous buyer approval\n    (buyer-approval invariant).\
  \ Agents unable to obtain approval at payment time must\n    route through the Shop skill (https://shop.app/SKILL.md) / Shop Pay.\ncontrols:\n  buyer_approval_invariant: true\n  rate_limited: true\n  rate_limit_signal: HTTP 429\n  recommended_skill: https://shop.app/SKILL.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chill/refs/heads/main/agentic-access/chill-agentic-access.yml
summary_line: 0 operations
tags:
- Company
- Wellness
- Supplements
- E-commerce
- Marketplace
- Health
- Agentic Commerce
- Shopify
- Retail
- MCP
---
