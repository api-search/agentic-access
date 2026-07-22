---
acting_count: 0
action_class_counts: {}
consequence_counts: {}
description: ''
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: searched
name: Source Beauty Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Source Beauty exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Source Beauty
provider_slug: source-beauty
slug: source-beauty-agentic-access
source_filename: source-beauty-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://sourcebeauty.com/llms.txt + https://sourcebeauty.com/.well-known/ucp\naudience: null\nsummary:\n  surface: Universal Commerce Protocol (UCP) shopping MCP + Shop skill\n  mcp_endpoint: https://sourcebeauty.com/api/ucp/mcp\n  human_in_the_loop_required: true\n  notes: >-\n    Source Beauty publishes explicit agent-access guidance (/llms.txt, mirrored at\n    /agents.md). Two sanctioned agent paths: (1) the store's own UCP shopping MCP\n    endpoint, (2) the cross-store Shop skill (https://shop.app/SKILL.md) routing\n    payment through Shop Pay. Published invariant: checkout MUST NOT complete payment\n    without contemporaneous, explicit buyer approval; agents must back off on HTTP 429.\noperations:\n- tool: search_catalog\n  action_class: read\n  consequence: read\n  human_in_the_loop: false\n- tool: create_cart\n  action_class: write\n  consequence: write\n  human_in_the_loop: false\n- tool: create_checkout\n  action_class:\
  \ acting\n  consequence: write\n  human_in_the_loop: false\n- tool: update_checkout\n  action_class: acting\n  consequence: write\n  human_in_the_loop: false\n- tool: complete_checkout\n  action_class: acting\n  consequence: physical\n  human_in_the_loop: required\n  rule: Buyer must explicitly approve payment at the moment of completion (published UCP rule).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/source-beauty/refs/heads/main/agentic-access/source-beauty-agentic-access.yml
summary_line: 5 operations · 1 human-in-the-loop
tags:
- Company
- Beauty
- Cosmetics
- E-commerce
- Retail
- Marketplace
- Wellness
- Egypt
- Skincare
- Consumer
---
