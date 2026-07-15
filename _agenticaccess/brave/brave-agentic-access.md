---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: brave-search-api.yml
  format: yaml
  label: Brave Search API
  slug: brave-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/openapi/brave-search-api.yml
- filename: brave-ads-api.yml
  format: yaml
  label: Brave Ads API
  slug: brave-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/openapi/brave-ads-api.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Brave Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Brave exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brave
provider_slug: brave
slug: brave-agentic-access
source_filename: brave-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/brave-ads-api.yml, openapi/brave-search-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/api/campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/report/campaign/csv/{campaignId}\n  method: get\n  operationId: getCampaignReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/search\n\
  \  method: get\n  operationId: webSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images/search\n  method: get\n  operationId: imageSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/search\n  method: get\n  operationId: videoSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news/search\n  method: get\n  operationId: newsSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggest/search\n  method: get\n  operationId: suggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /spellcheck/search\n  method: get\n  operationId: spellcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /local/pois\n  method: get\n  operationId: localPois\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /local/descriptions\n  method: get\n  operationId: localDescriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /web/rich\n  method: get\n  operationId: webRich\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/agentic-access/brave-agentic-access.yml
summary_line: 11 operations
tags:
- Search
- Advertising
- Privacy
- Browser
- AI
- LLM
---
