---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: theholisticcare-health-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Health API
  slug: theholisticcare-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-health-api-openapi.yml
- filename: theholisticcare-resources-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Resources API
  slug: theholisticcare-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-resources-api-openapi.yml
- filename: theholisticcare-search-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Search API
  slug: theholisticcare-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-search-api-openapi.yml
- filename: theholisticcare-blog-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Blog API
  slug: theholisticcare-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-blog-api-openapi.yml
- filename: theholisticcare-categories-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Categories API
  slug: theholisticcare-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-categories-api-openapi.yml
- filename: theholisticcare-glossary-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Glossary API
  slug: theholisticcare-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-glossary-api-openapi.yml
- filename: theholisticcare-mindfulness-games-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Mindfulness Games API
  slug: theholisticcare-mindfulness-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-mindfulness-games-api-openapi.yml
- filename: theholisticcare-panchavikas-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Panchavikas API
  slug: theholisticcare-panchavikas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-panchavikas-api-openapi.yml
- filename: theholisticcare-practices-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Practices API
  slug: theholisticcare-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-practices-api-openapi.yml
- filename: theholisticcare-whitepapers-api-openapi.yml
  format: yaml
  label: The Holistic Care — THC Open Mindfulness API Whitepapers API
  slug: theholisticcare-whitepapers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/openapi/theholisticcare-whitepapers-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Theholisticcare Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'The Holistic Care — THC Open Mindfulness API exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Holistic Care — THC Open Mindfulness API
provider_slug: theholisticcare
slug: theholisticcare-agentic-access
source_filename: theholisticcare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: generated\nsource: openapi/theholisticcare-blog-api-openapi.yml, openapi/theholisticcare-categories-api-openapi.yml,\n  openapi/theholisticcare-glossary-api-openapi.yml, openapi/theholisticcare-health-api-openapi.yml,\n  openapi/theholisticcare-mindfulness-games-api-openapi.yml, openapi/theholisticcare-panchavikas-api-openapi.yml,\n  openapi/theholisticcare-practices-api-openapi.yml, openapi/theholisticcare-resources-api-openapi.yml,\n  openapi/theholisticcare-search-api-openapi.yml, openapi/theholisticcare-whitepapers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path:\
  \ /v1/blog\n  method: get\n  operationId: getV1Blog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/blog/{slug}\n  method: get\n  operationId: getV1BlogBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/categories\n  method: get\n  operationId: getV1Categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/glossary\n  method: get\n  operationId: getV1Glossary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/glossary/{slug}\n  method: get\n  operationId: getV1GlossaryBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mindfulness-games\n  method: get\n  operationId: getV1MindfulnessGames\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mindfulness-games/{slug}\n  method: get\n  operationId: getV1MindfulnessGamesBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/panchavikas/resources\n  method: get\n  operationId: getV1PanchavikasResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/practices\n\
  \  method: get\n  operationId: getV1Practices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/practices/{slug}\n  method: get\n  operationId: getV1PracticesBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/resources\n  method: get\n  operationId: getV1Resources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: get\n  operationId: getV1Search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/whitepapers\n  method: get\n  operationId: getV1Whitepapers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/whitepapers/{slug}\n  method: get\n  operationId: getV1WhitepapersBySlug\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theholisticcare/refs/heads/main/agentic-access/theholisticcare-agentic-access.yml
summary_line: 15 operations
tags:
- Mindfulness
- Education
- Health
- OpenAPI
- Public APIs
- Free
---
