---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 11
api_specs:
- filename: agentic-news-ai-agents-api-openapi.yml
  format: yaml
  label: Agentic News Agents API
  slug: agentic-news-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-agents-api-openapi.yml
- filename: agentic-news-ai-api-keys-api-openapi.yml
  format: yaml
  label: Agentic News API Keys API
  slug: agentic-news-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-api-keys-api-openapi.yml
- filename: agentic-news-ai-briefing-api-openapi.yml
  format: yaml
  label: Agentic News Briefing API
  slug: agentic-news-ai-briefing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-briefing-api-openapi.yml
- filename: agentic-news-ai-feed-api-openapi.yml
  format: yaml
  label: Agentic News Feed API
  slug: agentic-news-ai-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-feed-api-openapi.yml
- filename: agentic-news-ai-search-api-openapi.yml
  format: yaml
  label: Agentic News Search API
  slug: agentic-news-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-search-api-openapi.yml
- filename: agentic-news-ai-stories-api-openapi.yml
  format: yaml
  label: Agentic News Stories API
  slug: agentic-news-ai-stories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-stories-api-openapi.yml
- filename: agentic-news-ai-trending-api-openapi.yml
  format: yaml
  label: Agentic News Trending API
  slug: agentic-news-ai-trending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-news-ai/openapi/agentic-news-ai-trending-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 1
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Agentic News Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api-keys/{id}
operation_count: 21
overview: 'Agentic News exposes 21 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 9 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentic News
provider_slug: agentic-news-ai
slug: agentic-news-ai-agentic-access
source_filename: agentic-news-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentic-news-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 11\n    acting: 10\n  by_consequence:\n    read: 11\n    write: 9\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /watches\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /watches\n  method: post\n  operationId: createAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /watches/{id}\n  method: patch\n  operationId: updateAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clusters/{id}\n  method: get\n  operationId: getStoryDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts/count\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /alerts/away-banner-shown\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/per-watch-unread-counts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alerts/{id}/read\n  method: post\n  operationId: markAlertRead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /alerts/{id}/read\n  method: delete\n  operationId: markAlertUnread\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /public/examples\n  method: get\n  operationId: getTrendingStories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/transparency\n  method: get\n  operationId: getTransparencyStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /briefing\n  method: get\n  operationId: getBriefing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-keys/{id}\n  method: delete\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /search\n  method: get\n  operationId: searchNews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agentic-news-ai/agentic-access/agentic-news-ai-agentic-access.yml
summary_line: 21 operations · 10 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- News
- Aggregation
- DailyBriefings
- AI Agents
---
