---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 12
api_specs:
- filename: lastminutedealshq-com-check-api-openapi.yml
  format: yaml
  label: lastminutedealshq-com Check API
  slug: lastminutedealshq-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastminutedealshq-com/openapi/lastminutedealshq-com-check-api-openapi.yml
- filename: lastminutedealshq-com-data-api-openapi.yml
  format: yaml
  label: lastminutedealshq-com Data API
  slug: lastminutedealshq-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastminutedealshq-com/openapi/lastminutedealshq-com-data-api-openapi.yml
- filename: lastminutedealshq-com-llms-txt-api-openapi.yml
  format: yaml
  label: lastminutedealshq-com Llms Txt API
  slug: lastminutedealshq-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastminutedealshq-com/openapi/lastminutedealshq-com-llms-txt-api-openapi.yml
- filename: lastminutedealshq-com-monitor-api-openapi.yml
  format: yaml
  label: lastminutedealshq-com Monitor API
  slug: lastminutedealshq-com-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastminutedealshq-com/openapi/lastminutedealshq-com-monitor-api-openapi.yml
- filename: lastminutedealshq-com-robots-lint-api-openapi.yml
  format: yaml
  label: lastminutedealshq-com Robots Lint API
  slug: lastminutedealshq-com-robots-lint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastminutedealshq-com/openapi/lastminutedealshq-com-robots-lint-api-openapi.yml
consequence_counts:
  read: 12
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lastminutedealshq Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'lastminutedealshq-com exposes 14 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: lastminutedealshq-com
provider_slug: lastminutedealshq-com
slug: lastminutedealshq-com-agentic-access
source_filename: lastminutedealshq-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/ai-visibility.lastminutedealshq.com-openapi.json, openapi/ai-visibility.lastminutedealshq.com_openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 12\n    acting: 2\n  by_consequence:\n    read: 12\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /check\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/llms-txt/generate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/llms-txt/validate\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/robots-lint\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/robots-lint\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/census.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/monitor\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /check\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/llms-txt/generate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/llms-txt/validate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/robots-lint\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/robots-lint\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/census.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/monitor\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/lastminutedealshq-com/agentic-access/lastminutedealshq-com-agentic-access.yml
summary_line: 14 operations · 2 acting
tags:
- Company
- Marketplace
- Deals
- E-Commerce
---
