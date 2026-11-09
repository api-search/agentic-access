---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: agenteconomy-cloud-aepi-api-openapi.yml
  format: yaml
  label: agenteconomy.cloud Aepi API
  slug: agenteconomy-cloud-aepi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenteconomy-cloud/openapi/agenteconomy-cloud-aepi-api-openapi.yml
- filename: agenteconomy-cloud-discovery-api-openapi.yml
  format: yaml
  label: agenteconomy.cloud Discovery API
  slug: agenteconomy-cloud-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenteconomy-cloud/openapi/agenteconomy-cloud-discovery-api-openapi.yml
- filename: agenteconomy-cloud-market-api-openapi.yml
  format: yaml
  label: agenteconomy.cloud Market API
  slug: agenteconomy-cloud-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenteconomy-cloud/openapi/agenteconomy-cloud-market-api-openapi.yml
- filename: agenteconomy-cloud-pricing-api-openapi.yml
  format: yaml
  label: agenteconomy.cloud Pricing API
  slug: agenteconomy-cloud-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenteconomy-cloud/openapi/agenteconomy-cloud-pricing-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agenteconomy Cloud Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'agenteconomy.cloud exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: agenteconomy.cloud
provider_slug: agenteconomy-cloud
slug: agenteconomy-cloud-agentic-access
source_filename: agenteconomy-cloud-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/agenteconomy-cloud-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: searchProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/{handle}\n  method: get\n  operationId: getProviderProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /compare\n  method: get\n  operationId: compareProviders\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alternatives\n  method: get\n  operationId: suggestAlternatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price\n  method: get\n  operationId: priceBenchmark\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price-index\n  method: get\n  operationId: getPriceIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /price-index/history\n  method: get\n  operationId: getPriceIndexHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /movers\n  method: get\n  operationId: movers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gaps\n  method: get\n  operationId: marketGaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /niche/{slug}\n  method: get\n  operationId: nicheReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demand\n  method: get\n  operationId: demandSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /indices\n  method: get\n  operationId: indices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agenteconomy-cloud/agentic-access/agenteconomy-cloud-agentic-access.yml
summary_line: 12 operations
tags:
- Artificial Intelligence
- Agents
- Economy
- Data
- Marketplace
---
