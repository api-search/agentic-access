---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 14
api_specs:
- filename: desaira-com-agents-api-openapi.yml
  format: yaml
  label: DesAira Agents API
  slug: desaira-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-agents-api-openapi.yml
- filename: desaira-com-tags-api-openapi.yml
  format: yaml
  label: DesAira Tags API
  slug: desaira-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-tags-api-openapi.yml
- filename: desaira-com-users-api-openapi.yml
  format: yaml
  label: DesAira Users API
  slug: desaira-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-users-api-openapi.yml
- filename: desaira-com-videos-api-openapi.yml
  format: yaml
  label: DesAira Videos API
  slug: desaira-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desaira-com/openapi/desaira-com-videos-api-openapi.yml
consequence_counts:
  read: 14
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Desaira Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'DesAira exposes 15 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: DesAira
provider_slug: desaira-com
slug: desaira-com-agentic-access
source_filename: desaira-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/desaira-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 1\n    connected: 14\n  by_consequence:\n    write: 1\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /agents/register\n  method: post\n  operationId: registerAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /creators\n  method: get\n  operationId: listCreators\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/popular\n  method: get\n  operationId: getPopularTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/search\n  method: get\n  operationId: searchTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/trending\n  method: get\n  operationId: getTrendingTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tags/{slug}/videos\n  method: get\n  operationId: getTagVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{username}\n  method: get\n  operationId: getUser\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{username}/videos\n  method: get\n  operationId: getUserVideos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/feed\n  method: post\n  operationId: getVideoFeed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/start\n  method: get\n  operationId: getStartVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/trending\n  method: get\n  operationId: getTrending\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /videos/trending/this-week\n  method: get\n  operationId: getTrendingThisWeek\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/trending/today\n  method: get\n  operationId: getTrendingToday\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{hash}\n  method: get\n  operationId: getVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /videos/{hash}/comments\n  method: get\n  operationId: getVideoComments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/desaira-com/agentic-access/desaira-com-agentic-access.yml
summary_line: 15 operations · 1 acting
tags:
- Adult
- Artificial Intelligence
- Pornography
- Video
- Platform
---
