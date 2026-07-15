---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 13
api_specs:
- filename: bored-api-openapi.yml
  format: yaml
  label: Bored API (Canonical)
  slug: bored-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/openapi/bored-api-openapi.yml
- filename: bored-appbrewery-openapi.yml
  format: yaml
  label: Bored API (App Brewery Community Fork)
  slug: bored-appbrewery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/openapi/bored-appbrewery-openapi.yml
consequence_counts:
  read: 13
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bored Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Bored API exposes 14 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bored API
provider_slug: bored
slug: bored-agentic-access
source_filename: bored-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bored-api-openapi.yml, openapi/bored-appbrewery-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 13\n    acting: 1\n  by_consequence:\n    read: 13\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/activity\n  method: get\n  operationId: getRandomActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/activity\n  method: get\n  operationId: getRandomActivityV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v2/activities\n  method: get\n  operationId: getRandomActivityV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/activities/{key}\n  method: get\n  operationId: getActivityByKeyV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/facts\n  method: get\n  operationId: getRandomFact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/facts/{key}\n  method: get\n  operationId: getFactByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/riddles\n  method: get\n  operationId: getRandomRiddle\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/riddles/{key}\n  method: get\n  operationId: getRiddleByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/websites\n  method: get\n  operationId: getRandomWebsite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/websites/{key}\n  method: get\n  operationId: getWebsiteByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/suggestions\n  method: post\n  operationId: submitSuggestion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /random\n  method: get\n  operationId: getRandom\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /filter\n  method: get\n  operationId: filterActivities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activity/{key}\n  method: get\n  operationId: getActivityByKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bored/refs/heads/main/agentic-access/bored-agentic-access.yml
summary_line: 14 operations · 1 acting
tags:
- Activities
- Boredom
- Community
- Development
- Discovery
- Education
- Facts
- Free
- MEVN
- No Auth
- Open Source
- Public APIs
- Recreation
- Riddles
- Suggestions
- Websites
---
