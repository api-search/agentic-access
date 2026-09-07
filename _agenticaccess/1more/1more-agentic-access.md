---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
consequence_counts:
  physical: 1
  read: 6
  write: 6
description: ''
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: 1More Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: '1MORE exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 6 write, and 1 physical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 1MORE
provider_slug: 1more
slug: 1more-agentic-access
source_filename: 1more-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: generated\nsource: mcp/1more-ucp-tools-list.json (probed tools/list, https://usa.1more.com/api/ucp/mcp) + https://usa.1more.com/agents.md\nnote: 'A recommended x-agentic-access execution contract for 1MORE''s agent commerce surface, classified\n  from the 13 real MCP tools the endpoint published. This is a governance STARTING POINT authored by API\n  Evangelist, not a claim 1MORE publishes it. One classification is NOT a heuristic: complete_checkout\n  is marked human-in-the-loop required because the store itself says so in its agents.md, and it is the\n  only tool that requires an idempotency key. audience is left null to bind per deployment. Derived from\n  OpenAPI is impossible here - there is no OpenAPI - so the tool input schemas are the authority for what\n  each operation takes.'\nsurface:\n  transport: mcp\n  endpoint: https://usa.1more.com/api/ucp/mcp\n  auth: none\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 6\n\
  \    acting: 7\n  by_consequence:\n    read: 6\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 1\noperations:\n- operation: get_checkout\n  action_class: connected\n  consequence: read\n  scope: order:read\n  token:\n    max_ttl_seconds: 3600\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: optional\n  audience: null\n- operation: create_checkout\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  token:\n    max_ttl_seconds: 900\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: required\n  audience: null\n- operation: update_checkout\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  token:\n    max_ttl_seconds: 900\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: required\n  audience: null\n- operation: complete_checkout\n  action_class: acting\n\
  \  consequence: physical\n  scope: checkout:complete\n  token:\n    max_ttl_seconds: 300\n    exchange: true\n    purpose_required: true\n  escalation:\n    human_in_the_loop: required\n    basis: 'Provider-stated, not inferred: https://usa.1more.com/agents.md - \"Checkout requires human\n      approval. Agents must not complete payment without explicit buyer consent.\"'\n  audit: required\n  idempotency:\n    required: true\n    field: meta.idempotency-key\n  audience: null\n- operation: cancel_checkout\n  action_class: acting\n  consequence: write\n  scope: checkout:write\n  token:\n    max_ttl_seconds: 900\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: required\n  audience: null\n- operation: get_cart\n  action_class: connected\n  consequence: read\n  scope: order:read\n  token:\n    max_ttl_seconds: 3600\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: optional\n\
  \  audience: null\n- operation: create_cart\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token:\n    max_ttl_seconds: 900\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: required\n  audience: null\n- operation: update_cart\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token:\n    max_ttl_seconds: 900\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: required\n  audience: null\n- operation: cancel_cart\n  action_class: acting\n  consequence: write\n  scope: cart:write\n  token:\n    max_ttl_seconds: 900\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: required\n  audience: null\n- operation: get_order\n  action_class: connected\n  consequence: read\n  scope: order:read\n  token:\n    max_ttl_seconds: 3600\n    exchange: false\n    purpose_required: false\n\
  \  escalation:\n    human_in_the_loop: not-required\n  audit: optional\n  audience: null\n- operation: search_catalog\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token:\n    max_ttl_seconds: 3600\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: optional\n  audience: null\n- operation: lookup_catalog\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token:\n    max_ttl_seconds: 3600\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: optional\n  audience: null\n- operation: get_product\n  action_class: connected\n  consequence: read\n  scope: catalog:read\n  token:\n    max_ttl_seconds: 3600\n    exchange: false\n    purpose_required: false\n  escalation:\n    human_in_the_loop: not-required\n  audit: optional\n  audience: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1more/refs/heads/main/agentic-access/1more-agentic-access.yml
summary_line: 13 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- Consumer Electronics
- Audio
- Headphones
- Retail
- E-Commerce
- Agent Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
---
