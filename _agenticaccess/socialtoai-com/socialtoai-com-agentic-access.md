---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 5
api_specs:
- filename: socialtoai-com-account-api-openapi.yml
  format: yaml
  label: socialtoai-com Account API
  slug: socialtoai-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-account-api-openapi.yml
- filename: socialtoai-com-call-api-openapi.yml
  format: yaml
  label: socialtoai-com Call API
  slug: socialtoai-com-call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-call-api-openapi.yml
- filename: socialtoai-com-capabilities-api-openapi.yml
  format: yaml
  label: socialtoai-com Capabilities API
  slug: socialtoai-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-capabilities-api-openapi.yml
- filename: socialtoai-com-comments-api-openapi.yml
  format: yaml
  label: socialtoai-com Comments API
  slug: socialtoai-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-comments-api-openapi.yml
- filename: socialtoai-com-detail-api-openapi.yml
  format: yaml
  label: socialtoai-com Detail API
  slug: socialtoai-com-detail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-detail-api-openapi.yml
- filename: socialtoai-com-find-api-openapi.yml
  format: yaml
  label: socialtoai-com Find API
  slug: socialtoai-com-find-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-find-api-openapi.yml
- filename: socialtoai-com-search-api-openapi.yml
  format: yaml
  label: socialtoai-com Search API
  slug: socialtoai-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-search-api-openapi.yml
- filename: socialtoai-com-trending-api-openapi.yml
  format: yaml
  label: socialtoai-com Trending API
  slug: socialtoai-com-trending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-trending-api-openapi.yml
- filename: socialtoai-com-user-posts-api-openapi.yml
  format: yaml
  label: socialtoai-com User Posts API
  slug: socialtoai-com-user-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-user-posts-api-openapi.yml
- filename: socialtoai-com-user-profile-api-openapi.yml
  format: yaml
  label: socialtoai-com User Profile API
  slug: socialtoai-com-user-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialtoai-com/openapi/socialtoai-com-user-profile-api-openapi.yml
consequence_counts:
  read: 5
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Socialtoai Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'socialtoai-com exposes 10 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: socialtoai-com
provider_slug: socialtoai-com
slug: socialtoai-com-agentic-access
source_filename: socialtoai-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/socialtoai-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 5\n    acting: 5\n  by_consequence:\n    read: 5\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trending\n  method: post\n  operationId: trending\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /detail\n  method: post\n  operationId: detail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /comments\n  method: post\n  operationId: comments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user_profile\n  method: post\n  operationId: user_profile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user_posts\n  method: post\n  operationId: user_posts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /call/{op}\n  method: post\n  operationId: call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /find\n  method: post\n  operationId: find\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities\n  method: get\n  operationId: capabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/socialtoai-com/agentic-access/socialtoai-com-agentic-access.yml
summary_line: 10 operations · 5 acting
tags:
- Company
- Social Media
- Artificial Intelligence
- Data API
- MCP
- Analytics
---
