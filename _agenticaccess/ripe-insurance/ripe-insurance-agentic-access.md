---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: ripe-insurance-content-api-openapi.yml
  format: yaml
  label: Ripe Insurance Content API
  slug: ripe-insurance-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-content-api-openapi.yml
- filename: ripe-insurance-media-api-openapi.yml
  format: yaml
  label: Ripe Insurance Media API
  slug: ripe-insurance-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-media-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ripe Insurance Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Ripe Insurance exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ripe Insurance
provider_slug: ripe-insurance
slug: ripe-insurance-agentic-access
source_filename: ripe-insurance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: generated\nsource: openapi/ripe-insurance-content-api-openapi.yml, openapi/ripe-insurance-media-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /umbraco/delivery/api/v1/content\n  method: get\n  operationId: GetContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/content\n  method: get\n  operationId: GetContent2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /umbraco/delivery/api/v1/content/item\n  method: get\n  operationId: GetContentItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v1/content/item/{path}\n  method: get\n  operationId: GetContentItemByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/content/item/{path}\n  method: get\n  operationId: GetContentItemByPath2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v1/content/item/{id}\n  method: get\n  operationId: GetContentItemById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /umbraco/delivery/api/v2/content/item/{id}\n  method: get\n  operationId: GetContentItemById2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/content/items\n  method: get\n  operationId: GetContentItems2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v1/media\n  method: get\n  operationId: GetMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/media\n  method: get\n  operationId: GetMedia2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v1/media/item\n\
  \  method: get\n  operationId: GetMediaItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v1/media/item/{path}\n  method: get\n  operationId: GetMediaItemByPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/media/item/{path}\n  method: get\n  operationId: GetMediaItemByPath2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v1/media/item/{id}\n  method: get\n  operationId: GetMediaItemById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/media/item/{id}\n  method: get\n\
  \  operationId: GetMediaItemById2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /umbraco/delivery/api/v2/media/items\n  method: get\n  operationId: GetMediaItems2.0\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/agentic-access/ripe-insurance-agentic-access.yml
summary_line: 16 operations
tags:
- Insurance
- United Kingdom
- Insurtech
- Managing General Agent
- Specialist Insurance
- Personal Lines
- Small Business Insurance
- Underwriting
- Direct to Consumer
- Brokers
---
