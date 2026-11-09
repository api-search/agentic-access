---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 5
api_specs:
- filename: githunt-ai-briefs-api-openapi.yml
  format: yaml
  label: githunt-ai Briefs API
  slug: githunt-ai-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-briefs-api-openapi.yml
- filename: githunt-ai-lists-api-openapi.yml
  format: yaml
  label: githunt-ai Lists API
  slug: githunt-ai-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-lists-api-openapi.yml
- filename: githunt-ai-profile-api-openapi.yml
  format: yaml
  label: githunt-ai Profile API
  slug: githunt-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-profile-api-openapi.yml
- filename: githunt-ai-search-api-openapi.yml
  format: yaml
  label: githunt-ai Search API
  slug: githunt-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-search-api-openapi.yml
- filename: githunt-ai-users-api-openapi.yml
  format: yaml
  label: githunt-ai Users API
  slug: githunt-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-users-api-openapi.yml
consequence_counts:
  read: 5
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Githunt Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'githunt-ai exposes 11 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: githunt-ai
provider_slug: githunt-ai
slug: githunt-ai-agentic-access
source_filename: githunt-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/githunt-ai-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 5\n    acting: 6\n  by_consequence:\n    read: 5\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search\n  method: post\n  operationId: searchDevelopers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/users/{login}\n  method: get\n  operationId: getDeveloper\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profile/analyze\n  method:\
  \ post\n  operationId: analyzeProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/users/{login}/evidence\n  method: get\n  operationId: getDeveloperEvidence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/briefs\n  method: post\n  operationId: createBrief\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/briefs/{briefId}\n  method: get\n  operationId: getBrief\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lists/{name}/logins\n  method: post\n  operationId: addSeenLogins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{name}/logins\n  method: delete\n  operationId: removeSeenLogins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{name}\n  method: get\n  operationId: getSeenList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/lists/{name}\n  method: delete\n  operationId: deleteSeenList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/lists/{name}/claims\n  method: post\n  operationId: claimSeenLogins\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/githunt-ai/agentic-access/githunt-ai-agentic-access.yml
summary_line: 11 operations · 6 acting
tags:
- Company
- Artificial Intelligence
- Talent
- Recruiting
- Developers
---
