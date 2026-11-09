---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: botfriendly-xyz-categories-api-openapi.yml
  format: yaml
  label: BotFriendly Categories API
  slug: botfriendly-xyz-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-categories-api-openapi.yml
- filename: botfriendly-xyz-check-api-openapi.yml
  format: yaml
  label: BotFriendly Check API
  slug: botfriendly-xyz-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-check-api-openapi.yml
- filename: botfriendly-xyz-featured-api-openapi.yml
  format: yaml
  label: BotFriendly Featured API
  slug: botfriendly-xyz-featured-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-featured-api-openapi.yml
- filename: botfriendly-xyz-health-api-openapi.yml
  format: yaml
  label: BotFriendly Health API
  slug: botfriendly-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-health-api-openapi.yml
- filename: botfriendly-xyz-protocols-api-openapi.yml
  format: yaml
  label: BotFriendly Protocols API
  slug: botfriendly-xyz-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-protocols-api-openapi.yml
- filename: botfriendly-xyz-search-api-openapi.yml
  format: yaml
  label: BotFriendly Search API
  slug: botfriendly-xyz-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-search-api-openapi.yml
- filename: botfriendly-xyz-services-api-openapi.yml
  format: yaml
  label: BotFriendly Services API
  slug: botfriendly-xyz-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-services-api-openapi.yml
- filename: botfriendly-xyz-stats-api-openapi.yml
  format: yaml
  label: BotFriendly Stats API
  slug: botfriendly-xyz-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-stats-api-openapi.yml
- filename: botfriendly-xyz-submissions-api-openapi.yml
  format: yaml
  label: BotFriendly Submissions API
  slug: botfriendly-xyz-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-submissions-api-openapi.yml
- filename: botfriendly-xyz-verify-api-openapi.yml
  format: yaml
  label: BotFriendly Verify API
  slug: botfriendly-xyz-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/botfriendly-xyz/openapi/botfriendly-xyz-verify-api-openapi.yml
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Botfriendly Xyz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'BotFriendly exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BotFriendly
provider_slug: botfriendly-xyz
slug: botfriendly-xyz-agentic-access
source_filename: botfriendly-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/botfriendly-xyz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /services\n  method: get\n  operationId: listServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /services/{slug}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId:\
  \ listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /featured\n  method: get\n  operationId: getFeatured\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /protocols\n  method: get\n  operationId: listProtocols\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify\n  method: post\n  operationId: verifyService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submissions\n  method: post\n  operationId: submitService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /search\n  method: get\n  operationId: searchServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /check\n  method: get\n  operationId: checkSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/botfriendly-xyz/agentic-access/botfriendly-xyz-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- BotFriendly
- AI Agents
- Machine-to-Machine
- API Directory
- OpenAPI
---
