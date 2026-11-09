---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 14
api_specs:
- filename: upspring-ai-ads-api-openapi.yml
  format: yaml
  label: upspring-ai Ads API
  slug: upspring-ai-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upspring-ai/openapi/upspring-ai-ads-api-openapi.yml
- filename: upspring-ai-advertisers-api-openapi.yml
  format: yaml
  label: upspring-ai Advertisers API
  slug: upspring-ai-advertisers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upspring-ai/openapi/upspring-ai-advertisers-api-openapi.yml
- filename: upspring-ai-docs-api-openapi.yml
  format: yaml
  label: upspring-ai Docs API
  slug: upspring-ai-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upspring-ai/openapi/upspring-ai-docs-api-openapi.yml
- filename: upspring-ai-taxonomy-api-openapi.yml
  format: yaml
  label: upspring-ai Taxonomy API
  slug: upspring-ai-taxonomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/upspring-ai/openapi/upspring-ai-taxonomy-api-openapi.yml
consequence_counts:
  read: 14
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Upspring Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'upspring-ai exposes 15 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: upspring-ai
provider_slug: upspring-ai
slug: upspring-ai-agentic-access
source_filename: upspring-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/upspring-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 14\n    acting: 1\n  by_consequence:\n    read: 14\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/ads\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ads/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ads/{id}/similar\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/advertisers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/advertisers/by-domain\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/advertisers/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/advertisers/{id}\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/advertisers/{id}/similar\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/advertisers/{id}/peers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/advertisers/{id}/compare/{otherId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/taxonomy/verticals\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/taxonomy/verticals/{vertical}/categories\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docs\n  method:\
  \ get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/docs/ui\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/upspring-ai/agentic-access/upspring-ai-agentic-access.yml
summary_line: 15 operations · 1 acting
tags:
- Advertising
- Artificial Intelligence
- Data
- Marketing
- Platform
---
