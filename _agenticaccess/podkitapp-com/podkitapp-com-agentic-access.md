---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: podkitapp-com-admin-api-openapi.yml
  format: yaml
  label: podkitapp-com Admin API
  slug: podkitapp-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-admin-api-openapi.yml
- filename: podkitapp-com-episodes-api-openapi.yml
  format: yaml
  label: podkitapp-com Episodes API
  slug: podkitapp-com-episodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-episodes-api-openapi.yml
- filename: podkitapp-com-podcasts-api-openapi.yml
  format: yaml
  label: podkitapp-com Podcasts API
  slug: podkitapp-com-podcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-podcasts-api-openapi.yml
- filename: podkitapp-com-search-api-openapi.yml
  format: yaml
  label: podkitapp-com Search API
  slug: podkitapp-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-search-api-openapi.yml
- filename: podkitapp-com-usage-api-openapi.yml
  format: yaml
  label: podkitapp-com Usage API
  slug: podkitapp-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/podkitapp-com/openapi/podkitapp-com-usage-api-openapi.yml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Podkitapp Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'podkitapp-com exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: podkitapp-com
provider_slug: podkitapp-com
slug: podkitapp-com-agentic-access
source_filename: podkitapp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/podkitapp-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/podcast/{itunesId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/episode/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/episode/{id}/chapters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/episode/{id}/transcript\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /admin/keys\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/podkitapp-com/agentic-access/podkitapp-com-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Podcasts
- Data
- Developers
- Audio
---
