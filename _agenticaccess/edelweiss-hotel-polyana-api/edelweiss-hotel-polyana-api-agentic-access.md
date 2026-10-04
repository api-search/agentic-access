---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: edelweiss-hotel-polyana-api-ai-llm-manifests-api-openapi.yml
  format: yaml
  label: Edelweiss Hotel Polyana API AI & LLM Manifests API
  slug: edelweiss-hotel-polyana-api-ai-llm-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edelweiss-hotel-polyana-api/refs/heads/main/openapi/edelweiss-hotel-polyana-api-ai-llm-manifests-api-openapi.yml
- filename: edelweiss-hotel-polyana-api-availability-pricing-api-openapi.yml
  format: yaml
  label: Edelweiss Hotel Polyana API Availability & Pricing API
  slug: edelweiss-hotel-polyana-api-availability-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edelweiss-hotel-polyana-api/refs/heads/main/openapi/edelweiss-hotel-polyana-api-availability-pricing-api-openapi.yml
- filename: edelweiss-hotel-polyana-api-hotel-information-api-openapi.yml
  format: yaml
  label: Edelweiss Hotel Polyana API Hotel Information API
  slug: edelweiss-hotel-polyana-api-hotel-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edelweiss-hotel-polyana-api/refs/heads/main/openapi/edelweiss-hotel-polyana-api-hotel-information-api-openapi.yml
- filename: edelweiss-hotel-polyana-api-search-api-openapi.yml
  format: yaml
  label: Edelweiss Hotel Polyana API Search API
  slug: edelweiss-hotel-polyana-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edelweiss-hotel-polyana-api/refs/heads/main/openapi/edelweiss-hotel-polyana-api-search-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Edelweiss Hotel Polyana Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Edelweiss Hotel Polyana API exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Edelweiss Hotel Polyana API
provider_slug: edelweiss-hotel-polyana-api
slug: edelweiss-hotel-polyana-api-agentic-access
source_filename: edelweiss-hotel-polyana-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: generated\nsource: openapi/edelweiss-hotel-polyana-api-ai-llm-manifests-api-openapi.yml, openapi/edelweiss-hotel-polyana-api-availability-pricing-api-openapi.yml,\n  openapi/edelweiss-hotel-polyana-api-hotel-information-api-openapi.yml, openapi/edelweiss-hotel-polyana-api-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/quote\n  method: get\n  operationId:\
  \ calculateStayQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/google-hotels/\n  method: get\n  operationId: getGoogleHotelsXml\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai-info/\n  method: get\n  operationId: getHotelAiInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: searchContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edelweiss-hotel-polyana-api/refs/heads/main/agentic-access/edelweiss-hotel-polyana-api-agentic-access.yml
summary_line: 5 operations
tags:
- Hotels
- Hospitality
- Travel
- Tourism
- Ukraine
- Carpathians
- Mineral Water
- Balneology
- Booking
- Room Rates
- google-hotels
---
