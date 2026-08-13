---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 4
consequence_counts:
  physical: 1
  read: 4
  write: 8
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Izotope Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'iZotope exposes 13 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: iZotope
provider_slug: izotope
slug: izotope-agentic-access
source_filename: izotope-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: generated\nsource: mcp/izotope-mcp-tools.json, https://www.izotope.com/llms.txt\nnote: >-\n  A recommended x-agentic-access execution contract per MCP tool, classified\n  from the live tool set at https://www.izotope.com/api/ucp/mcp. This is a\n  governance starting point produced by API Evangelist, not a claim iZotope\n  publishes — with one exception: the human-in-the-loop requirement on\n  complete_checkout is iZotope's own published rule (\"Checkout requires human\n  approval. Agents must not complete payment without explicit buyer consent.\"),\n  so it is recorded as provider-stated rather than recommended.\naudience: null\nsurface: https://www.izotope.com/api/ucp/mcp\nsummary:\n  operations: 13\n  by_action_class: {connected: 4, acting: 9}\n  by_consequence: {read: 4, write: 8, physical: 1}\n  human_in_the_loop: 1\n  provider_stated_controls: 1\noperations:\n  - operation: search_catalog\n    action_class: connected\n    consequence: read\n\
  \    scope: catalog:read\n    token: {ttl_seconds: 3600}\n    audit: optional\n  - operation: lookup_catalog\n    action_class: connected\n    consequence: read\n    scope: catalog:read\n    token: {ttl_seconds: 3600}\n    audit: optional\n  - operation: get_product\n    action_class: connected\n    consequence: read\n    scope: catalog:read\n    token: {ttl_seconds: 3600}\n    audit: optional\n  - operation: get_cart\n    action_class: connected\n    consequence: read\n    scope: cart:read\n    token: {ttl_seconds: 3600}\n    audit: optional\n  - operation: create_cart\n    action_class: acting\n    consequence: write\n    scope: cart:write\n    token: {ttl_seconds: 900}\n    audit: required\n  - operation: update_cart\n    action_class: acting\n    consequence: write\n    scope: cart:write\n    token: {ttl_seconds: 900}\n    audit: required\n  - operation: cancel_cart\n    action_class: acting\n    consequence: write\n    scope: cart:write\n    token: {ttl_seconds: 900}\n    audit: required\n\
  \  - operation: create_checkout\n    action_class: acting\n    consequence: write\n    scope: checkout:write\n    token: {ttl_seconds: 900}\n    audit: required\n    note: constructs a purchase intent but takes no payment\n  - operation: get_checkout\n    action_class: acting\n    consequence: write\n    scope: checkout:read\n    token: {ttl_seconds: 900}\n    audit: required\n    note: >-\n      classified acting rather than connected because the checkout object\n      carries buyer PII and payment instrument display data\n  - operation: update_checkout\n    action_class: acting\n    consequence: write\n    scope: checkout:write\n    token: {ttl_seconds: 900}\n    audit: required\n    note: accepts buyer email/phone, shipping destination and discount codes\n  - operation: cancel_checkout\n    action_class: acting\n    consequence: write\n    scope: checkout:write\n    token: {ttl_seconds: 900}\n    audit: required\n  - operation: get_order\n    action_class: acting\n    consequence: write\n\
  \    scope: order:read\n    token: {ttl_seconds: 900}\n    audit: required\n    note: returns a completed order including buyer and fulfillment detail\n  - operation: complete_checkout\n    action_class: acting\n    consequence: physical\n    scope: checkout:complete\n    token: {ttl_seconds: 300, exchange: true, purpose_required: true}\n    human_in_the_loop: required\n    human_in_the_loop_source: provider-stated\n    idempotency: {required: true, field: meta.idempotency-key}\n    audit: required\n    note: >-\n      Money moves and goods are licensed. iZotope's own llms.txt requires\n      contemporaneous buyer approval and directs agents that cannot obtain it\n      to route the purchase through Shop Pay instead of completing here.\nprovider_stated_rules:\n  - rule: Checkout requires human approval; agents must not complete payment without explicit buyer consent.\n    source: https://www.izotope.com/llms.txt\n  - rule: Respect rate limits; the MCP endpoint is rate-limited per IP, back\
  \ off on 429.\n    source: https://www.izotope.com/llms.txt\n  - rule: Pass context.address_country and context.currency for accurate pricing and availability.\n    source: https://www.izotope.com/llms.txt\n  - rule: Every tool call must identify the calling agent via meta.ucp-agent.profile.\n    source: mcp/izotope-mcp-tools.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/izotope/refs/heads/main/agentic-access/izotope-agentic-access.yml
summary_line: 13 operations · 9 acting
tags:
- Audio
- Audio Software
- Music Production
- Mixing
- Mastering
- Audio Restoration
- Audio Repair
- Post Production
- Plugins
- VST
- AudioUnit
- AAX
- DSP
- AI Audio
- Machine Learning Audio
- Vocal Processing
- Agent Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Ecommerce
- Boris FX
---
