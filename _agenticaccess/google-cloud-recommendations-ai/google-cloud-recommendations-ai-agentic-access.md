---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 1
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Cloud Recommendations AI API
  slug: google-cloud-recommendations-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-recommendations-ai/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Cloud Recommendations Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Google Cloud Recommendations AI exposes 4 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Cloud Recommendations AI
provider_slug: google-cloud-recommendations-ai
slug: google-cloud-recommendations-ai-agentic-access
source_filename: google-cloud-recommendations-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 1\n    acting: 3\n  by_consequence:\n    read: 1\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /projects/{projectId}/locations/{location}/catalogs/{catalogId}/catalogItems\n  method: get\n  operationId: listCatalogItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects/{projectId}/locations/{location}/catalogs/{catalogId}/catalogItems\n  method: post\n  operationId: createCatalogItem\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/locations/{location}/catalogs/{catalogId}/eventStores/{eventStoreId}/userEvents\n  method: post\n  operationId: writeUserEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /projects/{projectId}/locations/{location}/catalogs/{catalogId}/eventStores/{eventStoreId}/placements/{placementId}:predict\n  method: post\n  operationId: predict\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-recommendations-ai/refs/heads/main/agentic-access/google-cloud-recommendations-ai-agentic-access.yml
summary_line: 4 operations · 3 acting
tags:
- E-Commerce
- Google Cloud
- Machine Learning
- Personalization
- Recommendations
- Retail
---
