---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: apexai-academy-agents-api-openapi.yml
  format: yaml
  label: Apex AI Academy Agents API
  slug: apexai-academy-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-agents-api-openapi.yml
- filename: apexai-academy-courses-api-openapi.yml
  format: yaml
  label: Apex AI Academy Courses API
  slug: apexai-academy-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-courses-api-openapi.yml
- filename: apexai-academy-deep-dives-api-openapi.yml
  format: yaml
  label: Apex AI Academy Deep Dives API
  slug: apexai-academy-deep-dives-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-deep-dives-api-openapi.yml
- filename: apexai-academy-forum-api-openapi.yml
  format: yaml
  label: Apex AI Academy Forum API
  slug: apexai-academy-forum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-forum-api-openapi.yml
- filename: apexai-academy-lessons-api-openapi.yml
  format: yaml
  label: Apex AI Academy Lessons API
  slug: apexai-academy-lessons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-lessons-api-openapi.yml
- filename: apexai-academy-news-api-openapi.yml
  format: yaml
  label: Apex AI Academy News API
  slug: apexai-academy-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-news-api-openapi.yml
- filename: apexai-academy-pricing-api-openapi.yml
  format: yaml
  label: Apex AI Academy Pricing API
  slug: apexai-academy-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-pricing-api-openapi.yml
- filename: apexai-academy-search-api-openapi.yml
  format: yaml
  label: Apex AI Academy Search API
  slug: apexai-academy-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-search-api-openapi.yml
- filename: apexai-academy-subscribe-link-api-openapi.yml
  format: yaml
  label: Apex AI Academy Subscribe Link API
  slug: apexai-academy-subscribe-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apexai-academy/openapi/apexai-academy-subscribe-link-api-openapi.yml
consequence_counts:
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apexai Academy Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Apex AI Academy exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apex AI Academy
provider_slug: apexai-academy
slug: apexai-academy-agentic-access
source_filename: apexai-academy-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/apexai-academy-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 10\n    acting: 2\n  by_consequence:\n    read: 10\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /courses\n  method: get\n  operationId: list_courses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /courses/{course}/lessons\n  method: get\n  operationId: list_lessons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lessons/{slug}\n  method:\
  \ get\n  operationId: get_lesson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /news\n  method: get\n  operationId: latest_news\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deep-dives\n  method: get\n  operationId: list_deep_dives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pricing\n  method: get\n  operationId: get_pricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /subscribe-link\n  method: get\n  operationId: subscribe_link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agents/me/quiz\n  method: post\n  operationId: agent_quiz_answer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/forum/polls\n  method: get\n  operationId: forum_polls_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/forum/polls/{id}\n  method: get\n  operationId: forum_poll_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/forum/polls/{id}/vote\n  method: post\n  operationId: forum_poll_vote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/apexai-academy/agentic-access/apexai-academy-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Artificial Intelligence
- Education
- Learning
- Agents
- Platform
---
