---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: aipricinghub-com-changelog-api-openapi.yml
  format: yaml
  label: aipricinghub-com Changelog API
  slug: aipricinghub-com-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-changelog-api-openapi.yml
- filename: aipricinghub-com-freshness-api-openapi.yml
  format: yaml
  label: aipricinghub-com Freshness API
  slug: aipricinghub-com-freshness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-freshness-api-openapi.yml
- filename: aipricinghub-com-history-api-openapi.yml
  format: yaml
  label: aipricinghub-com History API
  slug: aipricinghub-com-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-history-api-openapi.yml
- filename: aipricinghub-com-industry-api-openapi.yml
  format: yaml
  label: aipricinghub-com Industry API
  slug: aipricinghub-com-industry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-industry-api-openapi.yml
- filename: aipricinghub-com-market-api-openapi.yml
  format: yaml
  label: aipricinghub-com Market API
  slug: aipricinghub-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-market-api-openapi.yml
- filename: aipricinghub-com-models-api-openapi.yml
  format: yaml
  label: aipricinghub-com Models API
  slug: aipricinghub-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-models-api-openapi.yml
- filename: aipricinghub-com-providers-api-openapi.yml
  format: yaml
  label: aipricinghub-com Providers API
  slug: aipricinghub-com-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-providers-api-openapi.yml
- filename: aipricinghub-com-rankings-api-openapi.yml
  format: yaml
  label: aipricinghub-com Rankings API
  slug: aipricinghub-com-rankings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aipricinghub-com/openapi/aipricinghub-com-rankings-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aipricinghub Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'aipricinghub-com exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: aipricinghub-com
provider_slug: aipricinghub-com
slug: aipricinghub-com-agentic-access
source_filename: aipricinghub-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/aipricinghub-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /providers\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /providers/{provider}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /models/{model}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rankings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rankings/{type}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history/{model}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /industry\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /freshness\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/aipricinghub-com/agentic-access/aipricinghub-com-agentic-access.yml
summary_line: 11 operations
tags:
- Artificial Intelligence
- Pricing
- Data
- Analytics
- Marketplace
- Comparison
---
