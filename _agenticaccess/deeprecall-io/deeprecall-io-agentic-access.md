---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: deeprecall-io-health-api-openapi.yml
  format: yaml
  label: DeepRecall Health API
  slug: deeprecall-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deeprecall-io/openapi/deeprecall-io-health-api-openapi.yml
- filename: deeprecall-io-recalls-api-openapi.yml
  format: yaml
  label: DeepRecall Recalls API
  slug: deeprecall-io-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deeprecall-io/openapi/deeprecall-io-recalls-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Deeprecall Io Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'DeepRecall exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DeepRecall
provider_slug: deeprecall-io
slug: deeprecall-io-agentic-access
source_filename: deeprecall-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/deeprecall-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/feed\n  method: get\n  operationId: get_recalls_feed_v1_recalls_feed_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/feed/{client}\n  method:\
  \ get\n  operationId: get_recalls_feed_for_client_v1_recalls_feed__client__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/sources\n  method: get\n  operationId: list_data_sources_v1_recalls_sources_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recalls/search\n  method: post\n  operationId: search_similar_recalls_v1_recalls_search_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/deeprecall-io/agentic-access/deeprecall-io-agentic-access.yml
summary_line: 5 operations
tags:
- Artificial Intelligence
- Regulatory
- Marketplace
- Compliance
- Intelligence
---
