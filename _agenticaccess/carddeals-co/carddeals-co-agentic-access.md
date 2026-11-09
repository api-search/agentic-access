---
acting_count: 0
action_class_counts:
  connected: 3
api_specs:
- filename: carddeals-co-gift-card-deals-api-openapi.yml
  format: yaml
  label: CardDeals Gift-card deals API
  slug: carddeals-co-gift-card-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carddeals-co/openapi/carddeals-co-gift-card-deals-api-openapi.yml
consequence_counts:
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Carddeals Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'CardDeals exposes 3 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CardDeals
provider_slug: carddeals-co
slug: carddeals-co-agentic-access
source_filename: carddeals-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/carddeals-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 3\n  by_consequence:\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/deals/search\n  method: get\n  operationId: searchGiftCardDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deals/lookup\n  method: get\n  operationId: lookupGiftCardDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deals/brands/{brand}\n  method: get\n  operationId:\
  \ getGiftCardDeals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/carddeals-co/agentic-access/carddeals-co-agentic-access.yml
summary_line: 3 operations
tags:
- Company
- Gift Cards
- Comparison
- Discounts
- E-Commerce
- Real-Time
---
